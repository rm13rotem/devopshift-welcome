# Dockerfile for Frontend Service
FROM python:3.12-slim

# Set working directory
WORKDIR /src
COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt
COPY . .

# Expose port 5002
EXPOSE 5002

CMD ["python", "main.py"]

