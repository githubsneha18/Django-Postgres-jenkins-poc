# Use an official Python runtime as a parent image
FROM python:3.x

# Set the working directory in the container
WORKDIR /app

# Copy the requirements file into the container and install dependencies
COPY requirements.txt .

# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Copy the rest of the application code into the container
COPY . .

# Start the Django application
CMD ["python", "manage.py", "runserver", "0.0.0.0:8000"]

