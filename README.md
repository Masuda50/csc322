# WhiteBoard - csc322 (Software Engineering) Final Project 

Contributors: Linda Li, Masuda Farehia, Yifeng Jin <GROUP J>

	Uses Python Flask and MYSQL

Summary: 
 
This website will facilitate an active teaming of people with similar interest and skill-set to forge groups for a certain do-good project.For a random visitor, the system provides a home page showcasing the top 3 rated projects and top rating OU profiles and SU profiles to showcase the power of the system. A visitor can surf around to find more OUs/VIPs and projects. Visitors also have the option to register to be an OU: If approved, they can login will a password sent to their email. If rejected, the applicant has one chance to appeal and the SU will make a final decision to reverse the rejection. OUs can form groups by inviting other OU(s) for a certain purpose: Once a group is formed, a group web-page should be made available that is accessible to all group members All group members can moderate and post to the group page. This page will be used for posting updates and scheduling meet-ups. An OU whose reputation score is higher than 30 will be promoted to VIP; and a VIP whose score is lower than 25 will be demoted. 

For a more indepth look into our system and its features, please take a look the the project specification, design documents, and diagrams included in this repository. 


How to run our system: 

System requirments: 

- Must have python version 2.7 or higher with its pip install feature 
- Install Flask (pip install Flask)
https://flask.palletsprojects.com/en/1.1.x/installation/
*** you can choose to run this project on a virutal env created on your computer but it is not required 
- Instal MYSQL Community Server and MYSQL Workbench (version 5.7)
https://dev.mysql.com/downloads/
video tutorial for reference: https://www.youtube.com/watch?v=UcpHkYfWarM&t=810s

Flask dependicies that must be installed: 

i. pip install flask_mail
ii. pip install flask_mysqldb 

1. Clone the master branch of this repo 
2. Once you have the MYSQL server running and you have created the root password, replace app.config['MYSQL_PASSWORD'] = 'xxxx' on line 35 of main.py with your root password 
3. Load the mysql script enclosed into your MYSQL workbench and click the lightning to load the script 
4. Once the tables and values are all loaded succesfully, in termial go into the cloned folder and run $python main.py 
5. Access MYSQL default localhost (usually localhost:5000) through a browser, which will load WhiteBoard for viewing purposes




================================================================================================================================

1. Clone this repository 

2. Run command: set FLASK_APP=main.py

3. Run command: set FLASK_DEBUG=1

4. Run command: flask run

5. In your browser head to http://localhost:5000/

6. Or run from PyCharm and go to browser

In doing so, any changes you make will be reflected upon refreshing the browser, that way you don't have to constantly restart the web server


**Used python program to design an web application with python flask and MYSQL**

# Requirements

  - Download and install Python, We used Python 3.7.1, make sure to check the box Add Python to PATH on the installation setup screen.
  - Download and install MySQL Community Server and MySQL Workbench, you can skip this step if you already have a MySQL server set up.
  - Install Python Flask with the command: pip install flask
  - Install Flask-MySQLdb with the command: pip install flask-mysqldb
  - ALSO, All requirements package will be on the requirements.txt and here is the references to check python flask installation: https://flask.palletsprojects.com/en/1.1.x/installation/

# File Structure & Setup
**Each file will contain the following:**
* \\-- vestigia
   <br> &emsp; &emsp;|-- main.py
  * &emsp;\\-- static
    <br> &emsp;&emsp; &emsp;|-- style.css
    <br> &emsp;&emsp; &emsp;|-- base.css
  * &emsp; \\-- templates
    <br> &emsp;&emsp; &emsp; |-- index.html
    <br> &emsp;&emsp; &emsp; |-- register.html
    <br> &emsp;&emsp; &emsp; |-- login.html
    <br> &emsp;&emsp; &emsp; |-- profile.html
    <br> &emsp;&emsp; &emsp; |-- layout.html 
    <br> &emsp;&emsp; &emsp; |-- reply.html 
    <br> &emsp;&emsp; &emsp; |-- post.html     
 -
  - main.py — This will be our main project file, all our Python code will be in this file (Routes, MySQL connection, validation, etc).
  - index.html — home page created with HTML5 and CSS3.
  - register.html — Registration form created with HTML5 and CSS3.
  - login.html — Login form created with HTML5 and CSS3.
  - profile.html - profile page created with HTML5 and CSS3.
  - post.html - post page created with HTML5 and CSS3.
  - reply.html - reply page created with HTML5 and CSS3.
  - layout.html - The layout template for the home and profile templates.

# The below instruction will start your web server (Windows):

- Make sure your MySQL server is up and running, it should have automatically started if you installed it via the installer.
- Make sure the database connection details below (in python) and your database should follow:
- app.secret_key = '111'
- app.config['MYSQL_HOST'] = 'localhost'
- app.config['MYSQL_USER'] = 'root'
- app.config['MYSQL_PASSWORD'] = '111111'
- app.config['MYSQL_DB'] = 'csc322_project'
- Open Command Prompt, make sure you have the project directory selected, you can do this with the command cd c:\your_project_folder_destination\python main.py on Windows.

# If you see the following information, you have successfully run the web application
* Serving Flask app "test" (lazy loading)
 * Environment: production
   WARNING: Do not use the development server in a production environment.
   Use a production WSGI server instead.
 * Debug mode: on
 * Restarting with stat
 * Debugger is active!
 * Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
# Click http://127.0.0.1:5000/ or copy it to your browser 
