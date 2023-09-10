### How to run on localhost?
- On MAC, CMD + P
- Rebuild Container
- Create a folder with kaggle credentials .kaggle/kaggle.json, which is required to get dataset from kaggle
- Terminal >> New Terminal
- mlflow ui
- In other terminal run experiments using command: 
mlflow run . --env-manager=local --experiment-name fraud -P n_trials=1

### Things to check after a successfull run
- After running command from terminal (mlflow ui), it should open a user interface under http://127.0.0.1:5000/#/experiments
- There should be data folder created within this project and following subfolders: raw, processed
- There should be a folder called mlruns within this project
- mlflow UI should contain experiments runs with predicted metrices generated using catboosting alogorithm
- There should be catboost_info folder generated within root director