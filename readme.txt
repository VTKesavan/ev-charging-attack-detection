# EV Attack Detection (AD-GS Framework)

- Project Overview

This project presents the AD-GS (Anomaly Detection - Global Security). framework, a comprehensive solution for identifying and mitigating cyber-attacks within Electric Vehicle (EV) charging infrastructures. The framework leverages a sophisticated ensemble of machine learning and deep learning models to detect a variety of attack vectors, including .DDoS, Data Manipulation, Man-in-the-Middle (MitM), False Data Injection (FDI), and Spoofing.. By analyzing charging session data, the AD-GS framework provides a robust defense mechanism to ensure the security and integrity of the EV charging ecosystem.

- Code Structure

The project is organized into a series of directories, each serving a specific purpose. The table below provides a summary of the key directories and their contents.

| Directory | Description |
|---|---|
| `Models/` | Contains pre-trained machine learning models in `.pkl` format, along with the data scaler used for preprocessing. |
| `Model_Results/` | Stores intermediate results from model training, including feature importance scores and model-specific configuration files. |
| `Processed_Data/` | Includes the datasets used for model training and evaluation, as well as visualizations generated during the analysis. |
| `Results/` | Contains the final evaluation reports, performance metrics, and statistical summaries of the dataset. |
| `anaconda_projects/` | Holds project-specific database files. |

- Getting Started

To get started with the AD-GS framework, you will need to set up your environment and run the main analysis script. The following sections provide detailed instructions on how to do so.

- Prerequisites

Before running the code, please ensure that you have Python installed on your system, along with the following libraries:

*   `tensorflow`
*   `scikit-learn`
*   `flwr`
*   `pandas`
*   `numpy`
*   `matplotlib`
*   `seaborn`
*   `xgboost`

- Execution

The core logic of the project is contained within the `Code_ev_attack_detection.ipynb` Jupyter Notebook. To run the analysis, follow these steps:

1.  .Launch Jupyter.: Open a terminal or command prompt and launch Jupyter Notebook or JupyterLab.
2.  .Open the Notebook.: Navigate to the project directory and open the `Code_ev_attack_detection.ipynb` notebook.
3.  .Run the Cells.: Execute the cells in the notebook sequentially. The notebook is divided into the following phases:
    -   .Phase 1.: Data analysis and statistical modeling.
    -   .Phase 2.: Development and training of the anomaly detection models.
    -   .Phase 3.: Simulation of a federated learning environment and integration of the ensemble model.
    -   .Phase 4.: Final evaluation of the models and visualization of the results.
4.  .Review the Results.: The final performance metrics and reports can be found in the `Results/` and `Model_Results/` directories.

- Implemented Models

The AD-GS framework incorporates a variety of models to ensure high-accuracy attack detection. The following table provides an overview of the models used in this project.

| Model | Description |
|---|---|
| .LSTM Autoencoder. | A deep learning model used for sequential anomaly detection based on reconstruction error. |
| .Random Forest. | A traditional machine learning classifier trained on tabular features. |
| .Support Vector Machine (SVM). | A model used for binary classification of normal versus attack-based charging sessions. |
| .Ensemble Model. | A model that combines the outputs from multiple models using a weighted voting scheme to improve overall accuracy. |
| .Federated Learning. | A decentralized training approach that simulates a real-world scenario with multiple charging stations, using the Flower framework. |

- Dataset

The data is labeled, with .0. indicating a normal session and .1. indicating an attack. The dataset is imbalanced, with a smaller proportion of attack samples. The attack types include DDoS, Data Manipulation, MitM, FDI, and Spoofing.
