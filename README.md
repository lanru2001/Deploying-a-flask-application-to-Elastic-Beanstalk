Flask is an open source web application framework for Python. This project is on Flask application and deploying it to an AWS Elastic Beanstalk environment.

1.Set up a Python virtual environment with flask:
Create a project directory and virtual environment for your application, and install Flask
mkdir flask_project && cd flask_project 

2.Create and activate a virtual environment named virt:
virtualenv virt && source virt/bin/activate

3.Install flask with pip install:
pip install flask==1.1.2

4.View the installed libraries with pip freeze:
pip freeze

5.Save the output from pip freeze to a file named requirements.txt:
pip freeze > requirements.txt

6.Create a new text file in this directory named application.py with the following contents:
Add the application.py code 

7.Run application.py with Python:
python application.py

8.Open  http://ip address:5000/ in your web browser. You should see the application running, showing the index page:

9.To create an environment and deploy your flask application:
eb init -p python-3.6 flask-tutorial --region us-east-2

#Optional 
10.Run eb init again to configure a default keypair so that you can connect to the EC2 instance running your application with SSH:
eb init

11.Create an environment and deploy your application to it with eb create:
eb create flask-env

12.When the environment creation process completes, open your web site with eb open:
eb open
