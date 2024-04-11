Voting Web Application using Django Framework

Introduction
votevista is a web application built using Django framework. It facilitates conducting polls consisting of questions and choices, allowing users to vote for their preferred choices. The application also provides result visualization for users to track the total votes for specific questions.

Implementation
Creating the Project
Setting Up the Environment:

Create an empty folder named votevista_project.
Set up a virtual environment using pipenv.
Install Django within the virtual environment.
Initializing Django Project:

Create a Django project named votevista.
Create an app named polls within the project.
Creating Models
Define Models:

Define two models, Question and Choice, in the models.py file.
Question contains fields for question text and publication date.
Choice contains fields for choice text, votes, and a foreign key relationship with Question.
Register Apps:

Include the polls app in the INSTALLED_APPS list in settings.py.
Migrations and Database Setup:

Generate and apply migrations to create database tables for models.
Creating Admin Interface
Create Superuser:

Create a superuser to access the admin panel.
Customize Admin Interface:

Customize admin site header, title, and index title.
Register models and inline choices for administration.
Creating Views
Define Views:

Implement views for displaying questions, voting, viewing details, and displaying results.
Utilize Django's built-in render function for rendering templates.
Define URLs:

Define URL patterns for views in the urls.py file within the polls app.
Creating Templates
Frontend Layout:

Create base HTML layout including navigation bar.
Create templates for index, detail, and results pages.
Configure Template Path:

Configure the template directory path in Django settings.
Creating Landing Page
Create Pages App:

Create a separate app named pages for the landing page.
Define Landing Page View and Template:

Implement a view to render the landing page.
Create an HTML template for the landing page.
Main URLs Configuration
Configure URLs:
Define URL patterns for both polls and pages apps in the main urls.py.
Testing
Admin Frontend
Admin Login:

Access the admin panel using the provided URL.
Log in using superuser credentials.
Add Questions:

Add questions and choices via the admin interface.
User Frontend
Access Landing Page:

Visit the landing page of the application.
Navigate to available polls.
Voting Process:

Select a question and vote for a choice.
View the voting results.
Future Scope
This project can serve as a foundation for implementing online voting systems in various domains. Future enhancements could include additional features based on specific requirements, such as user authentication, result analysis, and sharing options.

Quick Start
# Install dependencies
pip install pipenv

pipenv shell
# Install django
pipenv install django

cd votevista
# Serve on localhost:8000
python manage.py runserver
