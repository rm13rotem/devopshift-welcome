# Dockerfile for Backend Service
FROM python:3.12-slim
RUN pip install --upgrade pip
WORKDIR /src
# WORKDIR / failed

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .

# Expose port 5001
EXPOSE 5001

CMD ["python", "main.py"]

# Build your images locally from docker
# docker run -d -p 5002:5002 --name frontend-container my-frontend:1.0
# docker run -d -p 5001:5001 --name backend-container my-backend:1.0

