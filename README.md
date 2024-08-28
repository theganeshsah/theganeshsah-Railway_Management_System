# theganeshsah-Railway_Management_System

### Database Connection and Setup : 

The system first establishes a connection to a MySQL database and pyton using 
(
import mysql.connector
##### Establish a connection to the MySQL database
con = mysql.connector.connect(
    host="localhost",
    user="yourusername",
    password="yourpassword"
)
##### Create a cursor object
c = con.cursor()
).

after that create a database myrailway, if database exist then use it otherwise 
If the required database, named myrailway, doesn't exist, the system creates it. The database contains several key tables:

Train: Stores details about trains, including name, cost, distance covered, and date of travel.

Customer: Keeps records of customers, including their names, booked trains, payment amounts, travel dates, and contact information.

Bill: Tracks billing details.

Worker: Manages data about the railway workers, including their roles and salaries.


### System Password Login :

To ensure that only authorized personnel can manage the railway system, a password prompt is used. The correct password grants access to the system’s main options.

### Core Functionalities :

The RMS provides a variety of options for managing railway data:

Add Train: Input details for a new train and store them in the database.

Book Train: Record customer bookings and their associated details.

Add Bill: Manage and store billing information.

Add Worker: Enter details about workers, such as their roles and salaries.

View Data: Retrieve and display information from any of the tables.

### Managing Train Data

For example, adding a new train requires inputting the train’s name, cost, distance, and travel date. This information is stored in the Train table and can be retrieved or modified as needed.

### User Interface

The command-line interface is simple and intuitive, guiding users through each operation with clear prompts. After each operation, users are returned to the main menu, where they can choose their next task.

### In this project several SQL-related functions and methods are used to interact with the MySQL database.:

##### cursor()
It acts as a pointer that helps you interact with the database, execute commands, and retrieve data.

##### execute(sql_query, params=None)
To run SQL commands, such as SELECT, INSERT, UPDATE, DELETE, etc.

##### fetchall()
To retrieve and store all rows returned by a SQL query.

##### commit()
To finalize database transactions, ensuring that changes are saved permanently

##### close()
To properly close the connection to the database, avoiding potential issues like memory leaks or locked resources.




