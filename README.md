# Note-Keeper
**Overview:**
The Note Keeper application is a simple Java-based desktop tool designed to help users create, store, and search notes based on date or subject. It uses a MySQL database to store the notes.

**Features:**

1.Create Notes:

Users can create notes by entering the date, month, year, subject, and the note's text.

2.Search Notes by Date:

Users can search for notes by specifying the date, month, and year.

3.Search Notes by Subject:

Users can search for notes by specifying the subject.

**Technologies Used:**

1.Java AWT: For building the graphical user interface.

2.MySQL: Database management system to store notes.

3.JDBC (Java Database Connectivity): Connect Java applications with the MySQL database.

**Prerequisites:**

1.Java Development Kit (JDK)

2.MySQL Database

3.JDBC Driver for MySQL

**Setup Instructions:**

1.Database Setup:

Install MySQL:

Download and install MySQL from the official website.

Create Database and Table:

Open the MySQL command line or a database management tool

Create a new database and table using the following commands:

CREATE DATABASE notemaking;

USE notemaking;

CREATE TABLE notes (

    id INT AUTO_INCREMENT PRIMARY KEY,
    
    date VARCHAR(10),
    
    month VARCHAR(10),
    
    year VARCHAR(10),
    
    subject VARCHAR(100),
    
    text TEXT
    
);

2.Java Application Setup:

Clone the Repository:

Clone the project repository or copy the code into your local environment.

Add JDBC Driver to Classpath:

Download the JDBC Driver for MySQL from the official MySQL website.

Add the JDBC driver JAR file to the project's classpath.

Update Database Credentials:

Update the database connection credentials in the Note class:

private static final String URL = "jdbc:mysql://localhost:3306/notemaking";

private static final String USER = "root"; 

private static final String PASSWORD = "Suba@123"; 

Compile and Run the Application:

Compile the Java code using VS Code.

Run the Note class to start the application.

**Usage:**

Creating a Note:

Enter the date, month, year, subject, and note text in the provided fields.

Click the "CREATE" button to save the note to the database.

Searching for Notes by Date:

Enter the date, month, and year in the search fields.

Click the "DATE" button to search and display the notes for the specified date.

Searching for Notes by Subject:

Enter the subject in the search field.

Click the "SUBJECT" button to search and display the notes for the specified subject
