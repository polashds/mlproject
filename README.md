import dagshub
dagshub.init(repo_owner='polashds', repo_name='mlproject', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)


MLFLOW_TRACKING_URI=https://dagshub.com/polashds/mlproject.mlflow\
MLFLOW_TRACKING_USERNAME=polashds\
MLFLOW_TRACKING_PASSWORD=52f58776a97e4cde84895d1108511672\
python script.py