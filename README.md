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
