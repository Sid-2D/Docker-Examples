# Use python as base image
FROM python:2.7-slim

# Set working directory as /app
WORKDIR /app

# Copy current directory to /app
ADD . /app

# Install needed packages
RUN pip install -r requirements.txt

# Make port 80 available to outside
EXPOSE 80

# Define environment variable
ENV NAME World

# Run app.py when container launches
CMD ["python", "app.py"]