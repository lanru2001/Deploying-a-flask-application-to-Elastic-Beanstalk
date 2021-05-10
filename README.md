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

Run application.py with Python:
python application.py

Open  http://ip address:5000/ in your web browser. You should see the application running, showing the index page:

To create an environment and deploy your flask application:
eb init -p python-3.6 flask-tutorial --region us-east-2

#Optional 
Run eb init again to configure a default keypair so that you can connect to the EC2 instance running your application with SSH:
eb init

Create an environment and deploy your application to it with eb create:
eb create flask-env

When the environment creation process completes, open your web site with eb open:
eb open
