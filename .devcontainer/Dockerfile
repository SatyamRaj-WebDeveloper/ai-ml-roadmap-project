# Use an official Python image
FROM python:3.9-slim

# Set the working directory in the container
WORKDIR /app

# Install dependencies
# We copy *just* the requirements file first to use Docker's cache
COPY requirements.txt .
RUN pip install -r requirements.txt

# Copy the rest of the app
COPY . .

# This container will just sit and wait
CMD [ "sleep", "infinity" ]