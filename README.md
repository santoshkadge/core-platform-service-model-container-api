# Model-Container-API
This repository contains the model-container-api, a Python Flask-based microservice designed for executing machine learning models. It provides endpoints for executing models by their ID and version, both individually and in batches.

## Features
Execute machine learning models with specified parameters.
Support for both single execution and batch processing.
Role-based access control for model execution endpoints.
Integration with external services like AWS.
Customizable logging and error handling.

## Getting Started
These instructions will guide you through getting a copy of the project up and running on your local machine for development and testing purposes.

## Prerequisites
To install the software, you will need:

Python 3.9
pip
virtualenv (optional)
Installing

## Follow these steps to set up your development environment:

### Clone the Repository:

```
git clone https://yourrepositorylink.com/model-container-api.git
cd model-container-api
```

### Set Up a Python Virtual Environment (Optional but Recommended):
```
conda create -n model-container python=3.9
conda activate model-container
```

### Install the Required Dependencies:

```
pip install -r requirements.txt
```

### Set Up Environment Variables:

```
Copy the .env.example file to a new file named .env.
Edit .env with the values appropriate for your environment.
```

### Run the Application:

Run main.py by selecting "model-container" as the conda environment.
The API should now be accessible at http://localhost:5000.

### Usage
Here's how to use the service, including the available endpoints and how they can be accessed:

Example: Execute a Model
Request:

```
POST /model/{model_id}/{version}
Content-Type: application/json

{
  "param1": "value1",
  "param2": "value2"
}
```

Response:

```
{
  "result": "Execution result here"
}
```

## Running the Tests
Use pytest to run all the test cases. The conftest.py file in the tests directory includes fixtures for common setup, which provide a fixed baseline upon which tests can reliably and repeatedly execute.

## Deployment
Additional notes about deploying this on a live system can be added here.

## Built With
Flask - The web framework used.
Python - Programming language.


## Author
Santosh Kadge
