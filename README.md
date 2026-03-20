CREATE DATABASE company;
USE company;
CREATE TABLE Employee (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    department VARCHAR(50),
    salary FLOAT
);
CREATE TABLE Client (
    id INT PRIMARY KEY,
    name VARCHAR(50),
    project VARCHAR(50)
);
INSERT INTO Employee VALUES
(1, 'Amit', 'HR', 30000),
(2, 'Ravi', 'IT', 40000),
(3, 'Sita', 'Finance', 35000),
(4, 'Neha', 'Marketing', 32000),
(5, 'Raj', 'IT', 45000);
INSERT INTO Client VALUES
(1, 'ClientA', 'ProjectX'),
(2, 'ClientB', 'ProjectY'),
(3, 'ClientC', 'ProjectZ'),
(4, 'ClientD', 'ProjectA'),
(5, 'ClientE', 'ProjectB');
UPDATE Employee
SET salary = 50000
WHERE id = 2;
UPDATE Client
SET project = 'ProjectUpdated'
WHERE id = 3;
SELECT * FROM Employee;
SELECT * FROM Client;
