# Flask App with Docker and Kubernetes

This is a simple web application built using Flask and Docker. The app is containerized using Docker and deployed on Kubernetes for easy scaling and management.

## Technologies Used
- Python (Flask)
- Docker (for containerization)
- Kubernetes (for orchestration)
- GitHub (for version control)

## Installation

### Prerequisites
- Docker
- Kubernetes (Docker Desktop)
- Python

### Steps
1. Create a Github account and repository for the flask app:
    ```
    https://github.com/BRENDA-IMALINGAT/python-flask-project.git
    cd your-repository-name
    ```

2. install python flask:
   ```pip install flask```
   
4. create flask file
  ```app.py```
and import flask.

5. Install dependencies:
   requirements.txt
    ```bash
    pip install -r requirements.txt
    ```

6. Run the Flask app locally:
    ```bash
    python app.py
    ```
it should now be running on `http://localhost:5000`.

## Docker Setup
open docker desktop and login 

### Build the Docker Image
1. Build the Docker image:
    ```bash
    docker build -t assignment .
    ```

### Run the Docker Container
2. Run the Docker container:
    ```bash
    docker run -p 5000:5000 assignment
    ```
Flask app should be running on `http://localhost:5000`.

## Kubernetes Deployment

### Create Deployment and Service
create files: requirements.yaml and service.yaml
1. Apply the Kubernetes deployment:
    ```bash
    kubectl apply -f deployment.yaml
    ```

2. Expose the app using a service:
    ```bash
    kubectl apply -f service.yaml
    ```

### commit the files to the github respiratory
```bash
git init
git add .
git commit -m "initial commit"
git remote add origin https://github.com/BRENDA-IMALINGAT/python-flask-project.git
git push -u origin master```


