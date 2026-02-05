
README.txt
==========

Project Title:
EV Attack Detection System

Description:
This project contains source code and supporting scripts for detecting cyber/false data injection
and anomaly-based attacks in Electric Vehicle (EV) or Smart Grid environments using machine learning
and deep learning techniques.

The code is organized in a modular and hierarchical manner to support:
- Data preprocessing
- Feature extraction
- Model training and testing
- Performance evaluation
- Visualization and result analysis

Folder Hierarchy:
-----------------
ev_code/
  Code_ev-attack-detection/
    Code_ev_attack_detection.ipynb
    .ipynb_checkpoints/
      Code_ev_attack_detection.ipynb
    anaconda_projects/
      db/
        project_filebrowser.db
    Models/
      ad_gs_ensemble.pkl
      random_forest.pkl
      scaler.pkl
      svm_model.pkl
    Model_Results/
      ensemble_config.json
      feature_importance.csv
      federated_learning_results.json
      rf_results.json
      svm_results.json
    Processed_Data/
      attacked_dataset.csv
      attack_enriched_dataset.csv
      combined_data.csv
      features_dataset.csv
      Fig14.png
      Fig15.png
      Fig16.png
      Fig17.png
      Fig18.png
      preprocessed_dataset.csv
    Results/
      attack_specific_performance.json
      baseline_comparison.csv
      baseline_comparison.json
      confusion_matrices.json
      phase1_dataset_statistics.txt
      phase3_evaluation_report.txt
      phase3_metrics.json
      scalability_results.json
      visualization_data.json

How to Use the Code:
-------------------
1. Ensure Python 3.8 or above is installed.
2. Install required dependencies using:
   pip install -r requirements.txt   (if available)

3. Place the dataset (.csv format) in the appropriate data/ folder.
4. Run the main execution script (e.g., main.py or train.py) to:
   - Load and preprocess the dataset
   - Train the proposed attack detection model
   - Evaluate performance metrics

5. Use evaluation or plotting scripts to generate graphs and result tables.

Inputs:
-------
- Dataset file(s) in CSV format
- Configurable hyperparameters inside config or main scripts

Outputs:
--------
- Trained model files
- Performance metrics (Accuracy, Precision, Recall, F1-score, etc.)
- Graphs and plots for analysis

