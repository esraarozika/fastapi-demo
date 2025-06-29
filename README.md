# FastAPI Demo

A simple FastAPI web service with a `/hello` endpoint and Swagger documentation.

## How to Run

### Locally (No Docker)

pip install fastapi uvicorn
uvicorn app:app --reload

Visit: http://localhost:8000/hello?name=Essraa%20Hassanin

### In Docker

docker build -t fastapi-demo .
docker run -p 8000:8000 fastapi-demo

### Sample Output
Default response:
{ "message": "Hello, there!" }

Custom name response:
{ "message": "Hello, Essraa Hassanin!" }


### Docs
FastAPI auto-generates API docs:

Swagger UI: http://localhost:8000/docs

Redoc UI: http://localhost:8000/redoc
