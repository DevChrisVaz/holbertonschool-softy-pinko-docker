# Use the latest Ubuntu image
FROM ubuntu:latest

# Update APT and upgrade installed packages
RUN apt-get update && \
    apt-get upgrade -y

# Install Python 3, pip3, and dependencies
RUN apt-get install -y python3 python3-pip && \
    rm /usr/lib/python*/EXTERNALLY-MANAGED && \
    pip3 install flask flask-cors

# Set the working directory
WORKDIR /app

# Copy the Flask app into the container
COPY api.py /app/

# Expose the port the app runs on
EXPOSE 5252

# Run the Flask application
CMD ["python3", "api.py"]
