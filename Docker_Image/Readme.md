# Hospital Management System with AI Disease Prediction

A comprehensive hospital management system built with Flask, PostgreSQL, and machine learning capabilities for disease prediction based on patient symptoms.


## Features

- Patient Management: Complete CRUD operations for patient records
- Doctor Management: Manage doctor profiles, specializations, and availability
- Appointment Scheduling: Book, update, and track patient appointments
- AI-Powered Diagnosis: Machine learning model to predict diseases based on symptoms
- Disease Prediction API: Standalone endpoint for symptom-based disease prediction
- RESTful API: Clean and well-documented API endpoints
- Containerized Deployment: Docker and Docker Compose support
- Database Migrations: Flask-Migrate for database schema management



Start the application with docker

```bash
  cd Docker_Image
  docker compose build
  docker compose up
```


``
## Set Environment Variables

```bash
export FLASK_APP=run.py
export FLASK_ENV=development
export POSTGRES_HOST=db  # it is necessary for it to run with docker
export POSTGRES_PORT=5432
export POSTGRES_DB=hospital_app
export POSTGRES_USER=admin
``