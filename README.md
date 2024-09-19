# Database Systems Lab

Welcome to the Database Systems Lab repository! This repository contains notes, assignments, and syllabus details for the Database Systems Lab course.

## Contents

- **Notes:** Detailed notes covering key topics in Database Systems.
- **Assignments:** A collection of past assignments with questions and solutions.
- **Syllabus:** Comprehensive syllabus detailing the topics covered in the course.

## Syllabus

### Module 1: Data Definition and Data Manipulation Language
- Introduction to DDL (Data Definition Language) and DML (Data Manipulation Language)
- Creating, altering, and deleting database objects
- Inserting, updating, and deleting data

### Module 2: Constraints
- Types of constraints: Primary Key, Foreign Key, Unique, Not Null, Check
- Defining and enforcing constraints
- Role of constraints in maintaining data integrity

### Module 3: Single Row Functions
- Working with character, number, and date functions
- Conversion functions
- Null handling with functions

### Module 4: Operators and Group Functions
- Arithmetic, comparison, logical, and set operators
- Using aggregate functions: COUNT, SUM, AVG, MAX, MIN
- Grouping data with GROUP BY and HAVING clauses

### Module 5: Subqueries, Views, and Joins
- Writing single and multi-level subqueries
- Working with views: Creating, modifying, and deleting views
- Different types of joins: INNER, OUTER, SELF, and CROSS joins

### Module 6: High-Level Language Extensions
- Procedures: Creating and using stored procedures
- Functions: User-defined functions
- Cursors: Implicit and explicit cursors
- Triggers: Creating triggers for automatic execution based on data manipulation events

## Assignment Questions

1. Create tables identifying the primary keys and foreign keys, Insert necessary tuples into the table.

2. Enforce the Constraints
  
   a) The year of Date of Order should be below 2023.
   b) Customer Age Should be <100 and >17.
   c) The Default value of country is 'India'
   d) Alter the table to add the mobile number of customer table and its length should be 10.
   e) Customer name should be a Null Value.
   f) Add a Column email should be unique and can be null
   g) Add a Column Gender which could be any one of{'Male','Female', 'Trans')
   h) Enforce foreign key constraints as per the tables given with ON CASE CADE' feature.
   i) Rename the column named as 'amout' into 'Amount'
   j) add a column 'GST' into order table such that it store the percentage of GST tax (0.15 for 15%). The default % of GST is 8%.
  
3. Write SQL

  a) List the Customers whose name starts with ‘R’
  b) List the Customers whose age is >20 and <30.
  c) List the Foreign Customers and their email-ID
  d) Test the string manipulation functions – UPPER, LOWER, INITCAP, LENGTH, LPAD, RPAD, LTRIM, RTRIM and TRIM and NVL using select queries on data present in the tables. Use one query each for demonstration of one function
  e) Sort the List of Customers alphabetically
  f) List out the customer ID who have ordered the items on ’03-may-2023’
  g) List the customer Id who ordered the item where as its item cost >2000
  h) Calculate the GST amount based on the GST % for all items.
  i)Delete the orders with order-id 101
  j) Check the referential integrity during insertion / updation / Deletion of records of the table
  k) Update the Customer’s Country column by new value by replacing the old value
  l) Count and Display the number of customers
  m) Display the Names of customers grouped by country
  n) Count the No of customers from each country in descending order of the count
  o) Count the number of customers from ‘India’
  p) List out the count of customers in each country whereas the country should have minimum 5 customers
  q) List out the sum , avg, min max of all orders ordered
  r) Find out the Total Amount of all orders for each month of the year 2023
  s) Find out the average of sales of orders for each customer.
  t) Apply the multiple functions into a group by clause using any one of the table
  u) Apply the Nesting Aggregate Functions
  v) List out the customer id who have placed the order for more than one time
  w) Display the order-id sorted based on its amount
  x) Find out the months difference between two orders by customer id 102
  y) Display the Order date of each order in terms of its sentences
  z) Display the order date with YYYY-MM-DD HH24:MI:SS format

4. Assume the following relations:
    BOOKS(DocId, Title, Publisher, Year)
    STUDENTS(StId, StName, Major, Age)
    AUTHORS(AName, Address)
    Borrows (DocId, StId, Date)
    Has-written (DocId, AName)
    Describes (DocId, Keyword)

   Queries and Joins:
   List the year and title of each book.
   List all information about students whose major is CS.
   List all students with the books they can borrow.
   List all books published by McGraw-Hill before 1990.
   List the name of those authors who are living in Davis.
   List the name of students who are older than 30 and who are not studying CS.
   Rename AName in the relation AUTHORS to Name
   List the names of all students who have borrowed a book and who are CS majors.
   List the title of books written by the author 'Silberschatz'.
   List No books that have the keyword 'database'.
   Find the name of the youngest student.
   Find the title of the oldest book.
   List each book with its keywords.
   List each student with the books s/he has borrowed.
   List the title of books written by the author 'Ullman'.
   List the authors of the books the student 'Smith' has borrowed.
   Which books have both keywords 'database' and 'Programming'?

5. Assume Yourself at least 5 Non Correlated and 5 Correlated Sub-Query for the above Relational table and give your results

   Non-correlated Subqueries:
      1. Find the names of students who have borrowed at least one book
      2. Find the titles of books published after the year of the oldest book
      3. Find the names of authors who have written books with the keyword 'Science'
      4. Find the titles of books borrowed by students majoring in 'History'
      5. Find the names of students who have not borrowed any books

   Correlated Subqueries:
      1. Find the names of students who have borrowed books published by the same publisher as the book 'Database Systems'
      2. Find the names of students majoring in the same field as the student with the highest age
      3. Find the titles of books written by authors who live in the same city as the student 'John Doe'
      4. Find the names of authors who have written books borrowed by students majoring in 'Computer Science'
      5. Find the names of students who have borrowed books with the same keyword as their major


  6. Consider the following relational database of a college.
     Student(RollNumber, StudentName, Address)
     Teachers (TeacherID, TecherName, TeachingSubject)
     College(RollNumber, TeacherID)

   i) Create tables identifying the primary keys and foreign keys, Insert necessary tuples into the tables. (Min 5 rows)
   ii) Enforce the Constraints
   iii) Write SQL queries to find:
         a) Find the name of the Students who live in Chennai
         b) Find the name of the Teacher who teaches 'Cloud Computing' subject
         c) Find the Name of the teacher who teaches 'Java Programming' subject to the student 'Raman'
         d) List out the RollNo and Name who have enrolled with the teacher Name 'Radha Krishnan'


  7. PL/SQL Block For any GivenProject-ID, Display its Project_Name

  8. PL/SQL Block to delete a record from Department where there is no employee.

  9. PL/SQL Block to Update All Null valued Phone_no with “123456789”.

  10.  PL/SQL Block to count the total number of Employees working for the Given Project

  11.  Write a PL/SQL Procedure that will check for any updation of Project table such that the project title should not be started with “e-Commerce”.

  12.  Write a PL/SQL Function to count the Number of departments works for a Given Project-ID.

  13.  Use Cursor in PL/SQL Block to List out the Project Name and its Employee count for all projects.

  14.  Fire a Trigger during updation of Dept_ID in department table. The same dept-id should be reflected in employee table also.

  15.  Fire a Trigger during Insertion of any record into Project Table for ensuring the existence of its employee-id in employee table. Handle Exception if employee id is not available in the employee table.

  16.  Write a PL/SQL block to list the for each department name participating in the projects along with its total money spent for salary.
   

   
## Contributing

If you have any additional notes, assignments, or suggestions for the Database Systems Lab course, please get in touch. Your contributions are highly appreciated!

## Get in Touch! 📬

Feel free to reach out for:

- Any queries ❓
- Collaboration requests 🤝
- Study tips 📚
- Or just some tech talk! 💬

### Socials 📱

- **Twitter**: [@PajamaPadhai](https://twitter.com/PajamaPadhai)
- **Instagram**: [@PajamaPadhai](https://instagram.com/PajamaPadhai)

Or drop me an email at: **pajamapadhai@gmail.com**

---

Let’s dive into the world of databases and excel in our lab! Happy learning! 💾✨
