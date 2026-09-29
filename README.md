# answers.sql

-- WEEK 5 DATABASE ASSIGNMENT: INDEXING AND SECURITY


-- Question 1: Drop an index named IdxPhone from customers table
ALTER TABLE customers 
DROP INDEX IdxPhone;

-- Question 2: Create a user named bob restricted to localhost
CREATE USER 'bob'@'localhost' 
IDENTIFIED BY 'S$cu3r3!';

-- Question 3: Grant the INSERT privilege to bob on salesDB database
GRANT INSERT ON salesDB.* TO 'bob'@'localhost';

-- Question 4: Change the password for the user bob
ALTER USER 'bob'@'localhost' 
IDENTIFIED BY 'P$55!23';
