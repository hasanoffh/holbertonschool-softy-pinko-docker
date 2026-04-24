# Base image
FROM ubuntu:latest

# Update and Upgrade
RUN apt-get update && apt-get upgrade -y

# Install Python3, pip3
RUN apt-get install -y python3 python3-pip

# Fix for "externally managed" error
RUN rm -f /usr/lib/python*/EXTERNALLY-MANAGED

# Install Flask
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy the api.py to the working directory in the image
COPY api.py /app/api.py

# Command to run the Flask app
CMD ["python3", "api.py"]
