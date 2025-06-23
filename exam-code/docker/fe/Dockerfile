# Dockerfile for Frontend Service
FROM python:3.12-slim

# Set working directory
WORKDIR /app
#WORKDIR /src/templates failed

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY src/ ./src/
# Expose port 5002
EXPOSE 5002

CMD ["python", "src/main.py"]

#docker build -t my-frontend:1.4 ./fe
#docker build -t my-backend:1.4 ./be

#docker run -d -p 5002:5002 --name frontend-container my-frontend:1.4
#docker run -d -p 5001:5001 --name backend-container my-backend:1.4

#docker rm [container_id]
#docker rmi [image_id]

#docker images
#docker ps -a
#docker tag my-frontend:latest rm13rotem/project1:latest
#docker push rm13rotem/my-frontend:1.4