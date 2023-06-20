# collegeerp
Install the required modules using:
pip install -r requirements.txt

Run the following mysql commands before running the app
create database attendance_db;
CREATE TABLE notice (
  heading varchar(50) NOT NULL,
  actual varchar(16000) NOT NULL,
  n_id int NOT NULL,
  PRIMARY KEY (n_id)
);
INSERT INTO NOTICE(heading, actual, n_id) VALUES ("Welcome to TCET", "We welcome you,  AIML Batch of 2025 to Thakur College of Engineering and Technology", 1);
CREATE TABLE result (
  roll_no int NOT NULL,
  name varchar(45) NOT NULL,
  sdm varchar(45) NOT NULL,
  dsa varchar(45) NOT NULL,
  bai varchar(45) NOT NULL,
  dmbi varchar(45) NOT NULL,
  python varchar(45) NOT NULL,
  PRIMARY KEY (roll_no)
);
CREATE TABLE timetable (
  time varchar(50) NOT NULL,
  monday varchar(45) NOT NULL,
  tuesday varchar(45) NOT NULL,
  wednesday varchar(45) NOT NULL,
  thursday varchar(45) NOT NULL,
  friday varchar(45) NOT NULL
);
CREATE TABLE user (
  id int NOT NULL AUTO_INCREMENT,
  email varchar(150) DEFAULT NULL,
  password varchar(150) DEFAULT NULL,
  first_name varchar(150) DEFAULT NULL,
  contact_number int DEFAULT NULL,
  PRIMARY KEY (id),
  UNIQUE KEY email (email)
);
CREATE TABLE Student_Attendance_8(Roll_Number int, Name varchar(100));
INSERT INTO Student_Attendance_8 VALUES (1, "Ishaan Gupta"), (2, "Jihan Chheda"), (3, "Shrikar Gaikar"), (4, "Sahil Gupta"), (5, "Jayant Nag Sai Vasa"),
   (6, "Bhavya Jain"),(7, "Kunal Pawar"), (8, "Ishan Naik"),
   (, "Kartik Prajapati"), (10, "Akshay Vennikal");

