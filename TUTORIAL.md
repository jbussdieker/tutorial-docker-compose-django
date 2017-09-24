1. Create a Dockerfile

```
FROM python:3
ENV PYTHONUNBUFFERED 1
RUN mkdir /code
WORKDIR /code
ADD requirements.txt /code/
RUN pip install -r requirements.txt
ADD . /code/
```

2. Create requirements.txt

```
Django>=1.8,<2.0
psycopg2
```
