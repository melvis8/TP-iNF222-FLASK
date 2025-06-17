# Use the official Python base image
FROM python:3.10-slim

# Set environment variables
ENV PYTHONDONTWRITEBYTECODE=1
ENV PYTHONUNBUFFERED=1

# Set work directory
WORKDIR /app

RUN ls -la /app

# Install dependencies
COPY Docker_Image/requirements.txt .
COPY ../Code_Source ./Code_Source
RUN pip install --upgrade pip && pip install -r requirements.txt

# Copy project files
COPY . .

# Command to run the app
CMD ["python3", "Code_Source/app/run.py"]
