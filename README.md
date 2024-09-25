Library Management System

The goal of this project is to develop a comprehensive Library Management System that allows for efficient tracking and management of books, members, employees, and transactions within a library. This system facilitates operations like issuing and returning books, maintaining records of members, and generating reports for library management.

Database Structure

1    Database Creation 
    Created a database named Library_Management

2. Tables
   - Branch : Holds information about library branches, including branch ID, manager, address, and contact number.
   - Employees : Contains employee details, linking them to branches via foreign keys.
   - Members : Stores member information, including registration date and address.
   - Books : Details about books, such as ISBN, title, category, rental price, availability, author, and publisher.
   - Issued_Status : Records transactions of books issued, linking members and employees.
   - Return_Status : Tracks returned books, their condition, and links to issued records.

Key Features and Functionality

1. CRUD Operations:
   - Create : Added new book records and members using SQL `INSERT` commands.
   - Read : Utilized `SELECT` statements to retrieve data on books, members, branches, etc.
   - Update : Modified existing records, such as member addresses and book statuses using `UPDATE`.
   - Delete : Removed issued records when books were not returned.

2. Data Integrity:
   - Used foreign keys to maintain relationships between tables (e.g., linking issued books to members and employees).

3. Reporting and Analytics:
   - Created summary tables and reports:
     - Branch Performance Report : Showcases books issued, returned, and total revenue generated per branch.
     - Active Members : Identified members who issued books recently.
     - Book Rental Income : Analyzed income by book categories.
   
4.  Stored Procedures :
   - Developed stored procedures to automate processes:
     - Adding Return Records : Automates the process of logging returned books and updating their status.
     - Issuing Books : Checks book availability and manages the issuance process.

Advanced SQL Features

1. CTAS (Create Table As): 
   - Used to generate new tables based on query results, enhancing data analysis capabilities.

2. Group By and Aggregations:
   - Utilized to identify members who have issued multiple books and to calculate rental income.

3. Error Handling in Procedures:
   - Implemented logic to handle cases where a requested book is unavailable.

Challenges and Solutions

- Data Consistency: Ensured consistency through foreign key constraints, preventing orphan records.
- Complex Queries: Developed complex SQL queries for insights, such as overdue books and employee performance.

Conclusion 

This Library Management System streamlines library operations, enhances user experience, and provides valuable insights into library performance. Future enhancements could include a user-friendly interface, mobile access, and integration with online databases for book availability.

