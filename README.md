# Secure Login System with Multi-Factor Authentication

## Project Overview
A robust Django-based authentication system with advanced security features including Multi-Factor Authentication (MFA).

## Features
- Secure user registration
- Multi-Factor Authentication
- Advanced password validation
- Login attempt tracking
- Account lockout mechanisms

## Prerequisites
- Python 3.9+
- pip
- virtualenv (recommended)


**Create necessary directories:**

mkdir -p authentication/migrations
mkdir -p secure_login
mkdir -p templates/authentication
mkdir -p static/css
mkdir -p static/js
mkdir -p media


# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`

# Install dependencies
pip install -r requirements.txt

# Set up database
python manage.py makemigrations
python manage.py migrate

# Create superuser
python manage.py createsuperuser

# Run security tests
python MFA.py

# Start development server
python manage.py runserver