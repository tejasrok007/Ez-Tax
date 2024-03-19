# EasyTax
<p><b>Tax Management System</b> is a Java-based standalone application designed to help users efficiently manage their taxes and gain awareness about tax-saving opportunities. The project calculates taxes based on user inputs and provides valuable suggestions for tax optimization and appropriate investments. By utilizing this system, users can make informed financial decisions to improve their financial situation.</p>

## Table of Contents
1. [Introduction](#introduction)
2. [Features](#features)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Database Setup](#database-setup)


# Introduction
The purpose of the Tax Management System project is to simplify tax calculations and raise awareness among salaried individuals about potential tax-saving opportunities. By leveraging Java's AWT for the frontend and Java for the backend, this standalone application ensures a user-friendly experience for taxpayers.

# Features
<ol>
<li><b>Tax Calculation:</b> The application allows users to input their financial data and computes their tax liability based on the Indian taxation system.</li>
<li><b>Tax-saving Suggestions:</b> Users receive personalized suggestions on how to optimize their taxes and make suitable investments.</li>
<li><b>Educational Information:</b> Access to specific information about the Indian taxation system, helping users understand tax-related concepts better.</li>
<li><b>User-friendly Interface:</b> The AWT-based frontend provides an intuitive and visually appealing user interface.</li>
</ol>

# Installation
1. <b>Download and Install NetBeans IDE:</b>
If you haven't already installed NetBeans IDE, you can download it from the official website: NetBeans Downloads. Choose the appropriate version for your operating system and follow the installation instructions.

2. <b>Clone the Repository:</b>
Open a terminal or command prompt and navigate to the directory where you want to store the project. Then, use the following command to clone the repository:
bash
Copy code<br>
git clone https://github.com/pranavraikar01/EasyTaxD10AFinal.git

3. <b>Import the Project in NetBeans:</b>
Open NetBeans IDE and go to File > Open Project.... Navigate to the directory where you cloned the repository, select the project folder (EasyTax), and click "Open Project."

4. <b>Set Up MySQL Database:</b>
Ensure you have MySQL installed and set up the required database as mentioned in the Database Setup section of this README.

5. <b>Resolve Dependencies:</b>
If your project relies on external libraries or dependencies, ensure that you have added them to the project's classpath in NetBeans.

6. <b>Build and Run:</b>
Build the project in NetBeans by clicking on the "Build Project" button (hammer icon) or pressing F11. Once the build is successful, you can run the application by clicking on the "Run Project" button (green play icon) or pressing F6.
Note: Make sure to have the MySQL server running before running the application to avoid any connection issues.

Start Managing Your Taxes:
The Tax Management System application should now be up and running in NetBeans IDE. You can begin using it to manage your taxes efficiently.🎉🎉


# Usage
1. <b>Open the project.</b>
2. <b>Setup The MySQL database: </b>
Before running the application, ensure you have set up the required MySQL database as mentioned in the [Database Setup](#database-setup) section of this README.
3. <b>Login:</b>
Remember, This is a standalone project. Therefore, the login and password can be provided in the Java code once.
For now, Username is PRANAV, Password is 1234.
4. <b>Explore:</b>
Now, you are free to explore this project.

# Database Setup
1. Install MySQL database on your system. You can download it from MySQL Downloads.
2. Create a new database named "<b>EZTAX</b>" using the following SQL command:
CREATE DATABASE EZTAX;
3. Create a table called <b>user</b> which contains the information of users using the following SQL command:<br>
   CREATE TABLE user (
  name VARCHAR(255),
  panno VARCHAR(255),
  phoneno VARCHAR(255),
  income DECIMAL(10, 2),
  age INT,
  gender VARCHAR(10),
  HRA DECIMAL(10, 2),
  STANDARDDEDUCTIONS DECIMAL(10, 2),
  INTERESTONLOAN DECIMAL(10, 2),
  MEDICALINSURANCE DECIMAL(10, 2),
  DEDUCTIONONINVESTMENT DECIMAL(10, 2),
  NETTAX DECIMAL(10, 2)
);<br>
4. Last but not the least, replace the password with your MySQL password(which you set in while downloading MySQL) in  ./Project/ConnectionProvider.java .
