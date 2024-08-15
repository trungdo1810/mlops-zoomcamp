Sau khi tìm hiểu về build webserver bằng flask. Ta sẽ sử dụng MLFlow làm Model Registry để lưu models

- Nếu MLFlow đang chạy thì ta có thể get models từ `runs:/{RUN_ID}/model`

- Nếu MLFlow bị sập thì ta có thể tìm tới chỗ lưu models. Nếu ở local thì ở folder `/workspaces/mlops-zoomcamp/04-deployment/web-service-mlflow/mlflow/1/{RUN_ID}/artifacts/model`.
Nếu sử dụng cloud của Amazon thì lưu ở bucket S3