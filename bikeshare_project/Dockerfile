# Use an official Python runtime as a base image
FROM python:3.11

# Set the working directory in the container
# WORKDIR /app   


# Copy the requirements file   into the container at /app
COPY ./bikeshare_model_api /bikeshare_model_api/

# COPY requirements.txt /app/requirements.txt
WORKDIR /bikeshare_model_api
# Install any needed packages specified in requirements.txt
RUN pip install -r requirements.txt

# Make port 8001 available to the world outside this container
EXPOSE 8001

# Run the application using uvicorn
CMD ["python", "app/main.py"]