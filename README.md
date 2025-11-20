# RAGAPP

This is a minimal implementation of the RAG model for question answering.

# Requirements
* Python 3.8 or later
Install Python using MiniConda
1. Download and install MiniConda
2. Create a new environment using the following command:

* $ conda create -n <env-name> python=3.8
3.  Activate the environment
* $ conda activate <en-name>
4.  Install the required packages 
$ pip install -r requirements.txt

# Setup the environment variables
$ cp .env.example .env

Set your environment variables in the .env file. Like OPENAI_API_KEY value.

# Run Docker Compose Services
$ cd docker
$ cp .env.example .env

* update .env with your credentials

$ cd docker
$ sudo docker compose up -d

# Run the FastAPI server
$ uvicorn main:app --reload --host 0.0.0.0 --port 5000


