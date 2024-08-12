Email Microservice

Overview

This project is a POC microservice designed to handle the sending of emails and querying the statuses of sent emails.
We use AWS SES for email sending, AWS SNS for notification updates, and Amazon DynamoDB to store email data.

Project Structure

email-microservice/
├── app/
│   ├── __init__.py         # Initializes the Flask app and registers blueprints
│   ├── routes.py           # Defines the API endpoints for sending emails and checking statuses
│   ├── models.py           # Contains database models and schemas for DynamoDB (to be implemented)
├── venv/                   # Virtual environment directory
├── requirements.txt        # Python dependencies
├── run.py                  # Entry point to run the Flask application
├── README.md               # Project documentation
└── .gitignore              # Files and directories to be ignored by Git

Getting Started

Prerequisites

Python 3.x installed on your machine
Pip for managing Python packages
AWS CLI configured with access to DynamoDB, SES, and SNS
Git for version control

Run instructions

python run.py
http://127.0.0.1:5000/

POST /emails
GET /emails/:id/status
