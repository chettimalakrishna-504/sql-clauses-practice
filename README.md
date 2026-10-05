CREATE DATABASE query_builder;

USE query_builder;

CREATE TABLE users (
    id INT,
    name VARCHAR(100),
    age INT,
    city VARCHAR(100),
    salary INT
);

INSERT INTO users VALUES
(1, 'Krishna', 22, 'Hyderabad', 30000),
(2, 'Ravi', 25, 'Chennai', 40000),
(3, 'Suresh', 19, 'Hyderabad', 25000),
(4, 'Manoj', 30, 'Bangalore', 50000),
(5, 'Kiran', 17, 'Mumbai', 20000);

-- SELECT
SELECT id, name, age
FROM users;

-- Default SELECT *
SELECT *
FROM users;

-- WHERE
SELECT *
FROM users
WHERE age > 18;

-- Multiple WHERE conditions using AND
SELECT *
FROM users
WHERE age > 18
AND city = 'Hyderabad';

-- WHERE using OR
SELECT *
FROM users
WHERE age > 18
OR city = 'Hyderabad';

-- ORDER BY ASC
SELECT *
FROM users
ORDER BY name ASC;

-- ORDER BY DESC
SELECT *
FROM users
ORDER BY salary DESC;

-- Multiple ORDER BY
SELECT *
FROM users
ORDER BY city ASC, salary DESC;
