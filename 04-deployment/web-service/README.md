
gunicorn --bind=0.0.0.0:9696 predict:app

pipenv install --dev <pkg_1>

```bash
docker build -t ride-duration-prediction-service:v1 .
```


```bash
docker run -it --rm -p 9696:9696 ride-duration-prediction-service:v1
```