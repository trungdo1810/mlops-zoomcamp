## MLOPs 
Modules overview:

### 01. Introduction

### 02. Experiment tracking

- Experiment Tracker: Để thử nghiệm nhiều model ML, mỗi lần sửa và chạy Notebook ta sẽ thu được các (model, performance) --> lưu lại để so sánh các model với nhau    

- Model Registry: Sau khi train xong 1 model ML, ta cần save model. Nếu 1 model ML có nhiều option hyperparameter thì mỗi lần lưu ta phải đặt lại tên của model nếu không sẽ bị ghi đè file. 

### 03. Orchestration

Phần này sẽ học về cách sử dụng Mage để build data pipeline

### 04. Deployment

* Three ways of model deployment: Online (web and streaming) and offline (batch)
* Web service: model deployment with Flask
* Streaming: consuming events with AWS Kinesis and Lambda
* Batch: scoring data offline

### 05. Monitoring

* Monitoring ML-based services
* Monitoring web services with Prometheus, Evidently, and Grafana
* Monitoring batch jobs with Prefect, MongoDB, and Evidently