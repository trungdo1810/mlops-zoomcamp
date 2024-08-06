**Recap:**

now we hace the model  from module 3, operate, take the model and deploy

## Deployment Types:
There're **2 types/paradigms** of deployment

### **1. Offline (Batch mode)**

**Not real-time** prediction. Periodical prediction in hourly, daily, monthly. 

We have a **Database** and a **Scoring job(model)**. The Scoring job periodically pulls data from Database any time it requires and run the model on it. The result is written on a predictions DB.

Example: Churn job(dự đoán khả năng bỏ sử dụng dịch vụ để đưa ra các khuyến nghị, discount)

![offline.png](./images/offline.png)


### **2. Online**

The model is always available for prediction. There're **2 ways** to deploy an online model: **Web service** and **Streaming**.

- **Web service**

    + Periodical real-time forecasting(hourly, daily, monthly) depends on the interval set.
    + 1-1 relation ship (Backend - Model)

    Example: Taxi ride time prediction.

    ![webservice.png](./images/webservice.png)

- **Streaming**

**Note**: stream can be regarded as a agent, so both producers (who produce data) and consumers (who predict) **do not have direct connection but communicating via stream**.

+ We have a **producer(s)** and **consumers**. The producer pushes some data into a data stream and the consumers cna get the data for their tasks. 
+ 1-N relation ship 

Example: The backend (producer) pushes the data into the data stream alongside an event Ride_started; Consumer 1 (C1) predicts the duration, C2 predicts the cost, C3 predicts the Tip...etc

![streaming.png](./images/streaming.png)

Example:  A Youtuber update his/her content to the platform, the data can be sent to the stream, and the consumers (different models) can make a prediction based on the data obtained. The predictions are all sent to prediction stream and final decision could be sent to producer - remove or not remove the video (User).

![multi-stream.png](./images/multi-stream.png)

## Notes:
1. Offline: [Batch](https://github.com/Muhongfan/MLops/blob/main/04-deployment/Batch/REAMME.md)
2. Online:
   - Web service: 
     * [Web service](https://github.com/Muhongfan/MLops/blob/main/04-deployment/web-service/README.md)
     * [web-service-mlflow](https://github.com/Muhongfan/MLops/blob/main/04-deployment/web-service-mlflow/README.md)
   - Streaming:
     * [Streaming](https://github.com/Muhongfan/MLops/blob/main/04-deployment/streaming/README.md)