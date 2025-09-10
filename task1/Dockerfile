# Use the latest Ubuntu base image
FROM ubuntu:latest

# Update and upgrade packages
RUN apt-get update && apt-get upgrade -y

# Install Python3 and pip3
RUN apt-get install -y python3 python3-pip

# Fix "externally managed" restriction if it exists
RUN rm /usr/lib/python*/EXTERNALLY-MANAGED || true

# Install Flask via pip
RUN pip3 install flask

# Set working directory
WORKDIR /app

# Copy app code into the container
COPY api.py /app/

# Expose port 5252
EXPOSE 5252

# Run Flask app
CMD ["python3", "api.py"]
