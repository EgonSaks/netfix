# Netfix, service marketplace

![netfix](/img/netfix.webp)

## Overview

Netfix, service marketplace is a Django-based web application designed to connect service providers with customers in need. Through this platform, users can either offer or request a variety of services, ranging from home cleaning to carpentry. The aim is to create a one-stop solution for individuals to offer and avail different types of home and maintenance services.

## Tech Stack

- Language: Python
- Framework: Django (v4.2.5)
- Database: SQLite

## Installation

Ensure that you have Python 3.x installed on your machine. Clone the repository, navigate to the project directory, and install the required packages using the following commands:

```bash
git clone https://01.kood.tech/git/Egon/netfix
cd netfix
pip install -r requirements.txt
```

## Usage

To run the application, execute the following command in the project directory:

```bash
python3 -m venv env 
source env/bin/activate
python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py runserver
```

This will start the server on port 8000 by default in virtual environment.

## Features

### Core Features

- User Registration and Login:
  - Customers and Companies can register and login using their email and password.
  - Unique usernames and emails to avoid duplication.
  - Different registration fields for Customers and Companies.

- User Profiles:
  - Profile pages displaying user information.
  - List of requested services for Customers.
  - List of provided services and service creation option for Companies.

- Service Management:
  - Companies can create services based on their field of work.
  - Customers can request services by providing necessary details.
  - Service pages with detailed information and associated Company profile link.
  - Listing of services based on categories, creation time, and popularity.

- Miscellaneous:
  - Navigation bar for easy access to different sections.
  - Logout option for users.

## Structure

The project follows a typical Django project structure, with the main folder housing different apps for handling distinct aspects of the application:

- services: Manages service-related features.
- users: Manages user-related features.
- main: Manages common features across the project.

Each app contains essential Django files like **models.py** for database schema, **views.py** for backend logic, and **urls.py** for routing. Additionally, **forms.py** is used for form handling, and the **templates** directory is used for HTML templates.
