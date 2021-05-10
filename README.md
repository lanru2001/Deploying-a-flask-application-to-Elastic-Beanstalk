Flask is an open source web application framework for Python. This project is on Flask application and deploying it to an AWS Elastic Beanstalk environment.

Set up a Python virtual environment with flask:
1.Create a project directory and virtual environment for your application, and install Flask
mkdir flask_project && cd flask_project 

Create and activate a virtual environment named virt:
virtualenv virt && source virt/bin/activate

Install flask with pip install:
pip install flask==1.1.2

View the installed libraries with pip freeze:
pip freeze

Save the output from pip freeze to a file named requirements.txt:
pip freeze > requirements.txt

Create a new text file in this directory named application.py with the following contents:
Add the application.py code 
