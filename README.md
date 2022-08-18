# fastapi-example

A simple example of using Fast API in Python.

## Preconditions:

- Python 3

## Clone the project

```
git clone https://github.com/nguyenxuongkim2103/tdd-fastapi.git
```

## Run local

### Install dependencies

```
pip install -r requirements.txt
```

### Run server

```
uvicorn app.main:app --reload
```

### Run test

```
pytest app/test.py
```

### Run with Docker

Make sure Docker and Docker compose are installed.

Use Docker Compose to build a docker image from project's root folder:

```
$ docker compose build
```

Start docker container in detached mode:

```
$ docker compose up -d
```

Navigate to http://localhost:8004/ping. Make sure you see the same JSON response as before:

```json
{
  "ping": "pong!",
  "environment": "dev",
  "testing": false
}
```

## API documentation (provided by Swagger UI)

```
http://127.0.0.1:8000/docs
```

### Run server
