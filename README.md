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

pip install flask_mail
pip install flask_mysqldb 

1. Clone the master branch of this repo 
2. Once you have the MYSQL server running and you have created the root password, replace app.config['MYSQL_PASSWORD'] = 'xxxx' on line 35 of main.py with your root password 
3. Load the mysql script enclosed into your MYSQL workbench and click the lightning to load the script 
4. Once the tables and values are all loaded succesfully, in termial go into the cloned folder and run $python main.py 
5. Access MYSQL default localhost (usually localhost:5000) through a browser, which will load WhiteBoard for viewing purposes
