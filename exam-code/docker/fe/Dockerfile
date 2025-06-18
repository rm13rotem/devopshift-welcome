# Dockerfile for Frontend Service
FROM python:3.12-slim

# Set working directory
WORKDIR /src/templates
#WORKDIR /src failed

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .
# Expose port 5002
EXPOSE 5002

CMD ["python", "main.py"]

#docker build -t my-frontend:1.1 .

#docker run -p 5002:5002 my-frontend:1.1
#docker images
#docker ps -a
#docker tag my-frontend:latest rm13rotem/project1:latest
#docker push rm13rotem/my-frontend:1.1