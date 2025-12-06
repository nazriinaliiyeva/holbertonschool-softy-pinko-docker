# Use latest Ubuntu
FROM ubuntu:latest

# Update & upgrade APT
RUN apt-get update && apt-get upgrade -y

# Install Python & pip
RUN apt-get install -y python3 python3-pip

# Fix "externally-managed" issue
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask and CORS
RUN pip3 install flask flask-cors

# Work in /app
WORKDIR /app

# Copy API server
COPY ./api.py /app/api.py

# Run server
CMD ["python3", "/app/api.py"]

