# Use the latest Ubuntu image
FROM ubuntu:latest

# Update APT and upgrade installed packages
RUN apt-get update && \
    apt-get upgrade -y

# Clean up APT cache
RUN apt-get clean && \
    rm -rf /var/lib/apt/lists/*

# Set the default command to echo "Hello, World!"
CMD ["bash", "-c", "echo 'Hello, World!'"]