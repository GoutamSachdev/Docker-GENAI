# FastAPI with Hugging Face Transformers on Docker

This repository contains the code to deploy a FastAPI application that uses the Hugging Face Transformers library for text generation. The application is designed to be run inside a Docker container and can be easily deployed on platforms like Hugging Face Spaces.

## Directory Structure

- `app.py`: Contains the FastAPI application code.
- `Dockerfile`: Defines the Docker image.
- `requirements.txt`: Lists the Python dependencies.

## How to Build and Run

### Prerequisites

- Docker installed on your machine.
- Hugging Face account (optional for hosting on Hugging Face Spaces).

### Build Docker Image

Navigate to the directory containing the `Dockerfile` and run the following command:

```sh
docker build -t fastapi-transformers .
This will start the FastAPI application on http://0.0.0.0:7860.

Pushing to Hugging Face Spaces
Create a new space on Hugging Face.
Upload the app.py, Dockerfile, and requirements.txt files to the space.
Hugging Face Spaces will automatically build and deploy your application.
API Endpoints
GET /: Returns a welcome message.
GET /asking?text=<your_text>: Generates a text output based on the input text.
curl -X GET "http://0.0.0.0:7860/asking?text=Hello"

