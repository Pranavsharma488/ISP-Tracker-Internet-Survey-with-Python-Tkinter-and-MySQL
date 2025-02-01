NetInsight: ISP Survey System using Python Tkinter & MySQL

Overview

NetInsight is a GUI-based Internet Service Provider (ISP) survey system developed using Python Tkinter for the front-end and MySQL as the database. The system allows users to log in and submit survey responses about their internet usage, speed, and disruptions.

Features

-User Authentication: Secure login with predefined credentials.
-Survey Form: Collects user data on internet speed, ISP, and disruptions.
-MySQL Database Integration: Stores survey responses for analysis.
-GUI Interface: Built using Tkinter for a user-friendly experience.
-Error Handling: Provides alerts for missing fields or database errors.

Technologies Used

-Python (Tkinter for GUI)
-MySQL (Database for storing survey responses)
-MySQL Connector (To connect Python with MySQL)

Installation
-Prerequisites
Make sure you have the following installed on your system:
-Python 3.x
-MySQL Server
-Required Python libraries


Steps to Set Up

1.Install dependencies:
-pip install mysql-connector-python

2.Create MySQL Database and Table:
CREATE DATABASE registration;
CREATE TABLE survey_responses (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    age VARCHAR(20),
    state VARCHAR(50),
    isp VARCHAR(50),
    household VARCHAR(20),
    hours VARCHAR(20),
    download_speed VARCHAR(50),
    upload_speed VARCHAR(50),
    disruptions VARCHAR(10)
);

3.Update MySQL Credentials: Modify the connect_to_db() function in
  con = mysql.connector.connect(
            host="localhost",
            user="root",
            password="Jammu123@", 
            database="registration"  
        )

4.Run the application:
python main.py


Usage

-Run the script and log in with:
 Username: pranav
 Password: 123456

-Fill out the survey form and submit.
-The responses are stored in the MySQL database.





