# Final-Year-Project-Time-Series-Forecasting-with-VVIX-
## Project Overview
Volatility forecasting model evaluating VVIX and VIX dynamics using a hybrid ResNet-LSTM architecture and GAF/GADF feature representations.
This repository contains the source codes and technical documentation for the Final Year Project (CE301). This project focuses on forecasting the VVIX index (the Volatility of VIX index) through the use of multiple architectures, focusing on classical econometric models as well as advanced deep learning models.
Another core objective of this research is to apply explainable AI to the deep learning models through the use of Shapley Additive Explanations (SHAP) to provide explainability and transparency to these “black box” models that are typical of deep learning architectures.
## Key Features
•	Multi-model pipeline: implementation of classical econometric models (ARIMA and GARCH) and deep learning models (LSTM and XGBoost)
•	Interpretability: Optimised SHAP analysis with K-Means Clustering and Sample Capping for LSTM
•	Data Integrity: Implementation of strict data separation during the training and testing phases and iterative refinement to address scaling biases and data leakage.
•	Hybrid Transformation: Combining LSTM with Gramian Angular Fields (GAF) to transform 1D time-series data into 2D images for CNN-based processing through ResNet.
## Performance Results
Model	MSE	MAE	R2	Directional Accuracy
LSTM	0.0016	0.0283	0.8445	55.69%
GADF ResNet-LSTM	31.1274	3.8018	0.0488	54.79%
XGBoost	5.2018	1.3513	0.8433	42.52%
ARIMA	29.2026	3.5479	0.8906	48.18%
GARCH	5202.3529	28.9491	0.0346	45.16%

Only LSTM and the hybrid GADF ResNet-LSTM model surpassed the 50% mark for directional accuracy, making it useful for traders to know the direction of the price.

## Technical Stack
•	Environment: Python 3.x (Google Colab/GPU accelerated)
•	Deep Learning: TensorFlow, Keras
•	Machine Learning: XGBoost, Scikit-learn
•	Explainability: SHAP
•	Data Manipulation: Pandas, NumPy
•	Visualisation: Matplotlib, Seaborn
## Repository Structure
•	/datasets: where the dataset was kept.
•	/pythonfiles: all the Python notebooks that were used for this project.
•	/results: Visualisations, including SHAP summary graphs, and Actual vs. Predicted graphs.
•	README.md: Technical documentation on the report.
## Project Management
Project management for this final year project was handled through Kanban in Tuleap, documenting research, implementation and refinement.
## Author
Adruce bin Khairudin
University of Essex
CE301, Final Year Project
## License
This project is intended for academic evaluation and is not for commercial financial use.

