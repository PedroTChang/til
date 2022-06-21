# SQL Search Reference & Exercise

### Reference:

SELECT \* FROM recipes
WHERE prep_time > 100
AND ingredients LIKE '%bread%'
ORDER BY prep_time DESC
LIMIT 2;

### Exercise:

Use SQL to grab the following data from the employees database:

1. Get all info about employees whose last names begin with “Z”.
   SELECT \* FROM employees WHERE last_name LIKE 'Z%'
2. Get the first name and last name of employees whose last names begin with “Mi”.
   SELECT first_name, last_name FROM employees WHERE last_name LIKE 'Mi%'
3. Get the first name, last name, and birthday of 5 eldest employees.
   SELECT first_name, last_name, birth_date FROM employees ORDER BY birth_date LIMIT 5;
4. Get all info about the 5 most recent hires.
   SELECT \* FROM employees ORDER BY hire_date DESC LIMIT 5;
5. Get all info about 5 most recent female hires.
   SELECT \* FROM employees WHERE gender = 'F' ORDER BY hire_date DESC LIMIT 5;
6. Bonus: Get all the info on all employees whose first name is Mario or Luigi.
   SELECT \* FROM employees WHERE first_name = 'Mario' OR first_name = 'Luigi'
7. Bonus: Get only the first and last name of employees without the last name “Aingworth.”

8. Bonus: Get all the info on employees whose first name is Arif, but only those hired between 1988 and 1992.

9. Bonus: How many employees were making over $100,000 a year on June 24, 1992? Return only a number.

10. Bonus: Repeat exercise #2 without using the LIKE keyword.

11. Uber bonus: Research how to do a case-insensitive search in postgres and try it out in Postico (there is more than one way…)
