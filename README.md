https://dagshub.com/kanthibushan/mlflow_demo.mlflow
import dagshub
dagshub.init(repo_owner='kanthibushan', repo_name='mlflow_demo', mlflow=True)

import mlflow
with mlflow.start_run():
  mlflow.log_param('parameter name', 'value')
  mlflow.log_metric('metric name', 1)