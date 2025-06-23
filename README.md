# Flask Docker App

This is a simple Flask web application that runs inside a Docker container. It's designed for beginners to learn the basics of containerizing a Python web app using Docker.

## 🚀 Features

* Python Flask web server
* Dockerized with a clean Dockerfile
* Serves a basic "Hello World" response
* Easy to build and run on any system with Docker

## 🛠️ Tech Stack

* Python 3.10
* Flask
* Docker

## 📁 Project Structure

```
flask-docker-app/
├── app.py               # Flask application
├── requirements.txt     # Python dependencies
└── Dockerfile           # Docker configuration
```

## 🧪 How to Run This Project

### 1. Clone the repository

```bash
git clone https://github.com/your-username/flask-docker-app.git
cd flask-docker-app
```

### 2. Build the Docker image

```bash
docker build -t flask-demo .
```

### 3. Run the Docker container

```bash
docker run -p 5000:5000 flask-demo
```

If port 5000 is busy, try:

```bash
docker run -p 5001:5000 flask-demo
```

### 4. View the App

Visit [http://localhost:5000](http://localhost:5000) (or [http://localhost:5001](http://localhost:5001)) in your browser.

You should see:

🔥 Hello from your first Flask app!

## 📄 app.py Contents

```python
from flask import Flask

app = Flask(__name__)

@app.route('/')
def home():
    return "🔥 Hello from your first Flask app!"

if __name__ == '__main__':
    app.run(host='0.0.0.0', port=5000)
```


Created by Antony Varghese — built for learning Flask and Docker.

---
