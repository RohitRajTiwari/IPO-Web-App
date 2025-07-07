# IPO-Web-App
IPO WEB APPLICATION BY BLUESTOCK FINTECH
# 🧾 Bluestock IPO Web App

This project is a full-stack Django + React-based IPO management system developed for Bluestock Fintech.

---
| Name                 | Role                            | GitHub Profile                                            |
| -------------------- | ------------------------------- | --------------------------------------------------------- |
| **Rohit Raj Tiwari** | Frontend Developer              | https://github.com/RohitRajTiwari |
| **Astha Dahiya**     | Team Leader & Backend Developer | (https://github.com/Astha2004-a)                  |



Setup PostgreSQL Database
✅ Prerequisite: Install PostgreSQL
Download and install PostgreSQL from the official website:
👉 https://www.postgresql.org/download/

✅ Create Database and User
Open PostgreSQL terminal (psql) and run:
CREATE DATABASE bluestock;
CREATE USER daiyanalam WITH PASSWORD '12345';
ALTER ROLE daiyanalam SET client_encoding TO 'utf8';
ALTER ROLE daiyanalam SET default_transaction_isolation TO 'read committed';
ALTER ROLE daiyanalam SET timezone TO 'UTC';
GRANT ALL PRIVILEGES ON DATABASE bluestock TO daiyanalam;


 Install PostgreSQL Adapter for Python

 pip install psycopg2-binary


Configure Django to use PostgreSQL

In bluestock/settings.py, update the DATABASES section:

DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'bluestock',
        'USER': 'daiyanalam',
        'PASSWORD': '12345',
        'HOST': 'localhost',
        'PORT': '5432',
    }
}

Run Migrations and Start Server

python3 manage.py makemigrations
python3 manage.py migrate
python3 manage.py createsuperuser
python3 manage.py runserver





