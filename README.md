# Tourism Ecosystem Platform
Tourism Ecosystem microservices (Tour, Room, and Ride booking) were implemented while completing the Service-Oriented Software Engineering course.

# About the project:
This project is a Tourism Ecosystem Platform that allows users to book tours, rooms, and rides using a microservices architecture. The system integrates third-party payment services, sends notifications via email/SMS, and provides event log analytics for process improvements.

# Technologies Used:
    - Python (Flask) - Backend framework
    - MySQL - Database
    - HTML/CSS/JavaScript - Frontend
    - Stripe - Payment processing
    - Mailtrap - Email services
    - Twilio - SMS notifications


# Installation
## Prerequisites before running app.py file:
    1. Python 3.x installed
    2. For database integration, install MySQL workbench and community editions accordingly in your pc. Afterwards, configure your MySQL credentials in the python file.

## Create a virtual environment (optional):
python -m venv venv
source venv/bin/activate  # For Windows use: venv\Scripts\activate

## Install Dependencies
    1. pip install Flask
    2. pip install flask-mysqldb
    3. pip install stripe
    4. pip install flask-mail  # For email
    5. pip install twilio      # For SMS
    6. pip install smtplib

## Configure app.py file with API keys & database credentials
    1. For payment system integration, create an account in Stripe. Afterwards, configure the stripe secret api key of your profile.
    2. For Email sending functionality, create an account in Mailtrap. Afterwards, configure the mailtrap credentials (host, port, username, password).
    3. For SMS sending functionality, create an account in Twilio. Afterwards, configure the twilio credentials (account sid, auth token, free trial number as sender number).

Note: In the current code (app.py), the corresponding credentials are masked with asterisks (*). Make sure to add your own credentials before running the project.

# Integrate with Database
    1. Connect to MySQL server in Workbench by providing username and password of your localhost
    2. Run db.sql file to create database with necessary tables and data

# Running the Project
    1. Start the Flask server by running app.py python file
    2. Access the Tour booking application at http://127.0.0.1:5000 (Tour Booking Form)
    3. Access Room booking form at http://127.0.0.1:5000/room_booking
    4. Access Ride booking form at http://127.0.0.1:5000/ride_booking

