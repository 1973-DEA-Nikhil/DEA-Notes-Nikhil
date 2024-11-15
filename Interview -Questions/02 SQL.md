### SQL INTERVIEW QUESTIONS

#### Basic SQL Questions

1. **DDL & DML**
   - "What is the difference between DDL and DML? Provide examples of each."
   - "How do you rename a table in SQL?"
   - "Write a query to rename a column in a table."
   - "What are the different types of indexes in SQL?"

2. **Data Types & Constraints**
   - "What is the difference between CHAR and VARCHAR?"
   - "What is a PRIMARY KEY? What is an ALTERNATIVE KEY?"
   - "How much storage does CHAR(10) take versus VARCHAR(10)?"
   - "What are the different constraints you can apply to a column?"

3. **Normalization**
   - "Explain the different normal forms in database normalization."
   - "Given this table structure, identify normalization issues and how to fix them:
     ```sql
     Orders(order_id, customer_name, customer_address, product1, price1, product2, price2)
     ```
   "

#### Query-Based Questions

1. **Basic Queries**
   ```sql
   -- Write a query to find employees in HR department with salary above 50,000
   -- Tables: employees(emp_id, name, dept_id, salary), departments(dept_id, dept_name)
   ```

2. **Aggregation & Grouping**
   ```sql
   -- Write a query to find the number of employees in each department
   -- Tables: employees(emp_id, name, dept_id)
   ```

   ```sql
   -- Find the average salary for each department
   -- Exclude employees who have salary greater than company average
   ```

3. **Join Operations**
   ```sql
   -- Write a query to find all employees and their managers, including employees with no manager
   -- Table: employees(emp_id, name, manager_id)
   ```

4. **Highest Salary Queries**
   ```sql
   -- Write a query to find the 3rd highest salary
   -- Table: employees(emp_id, name, salary)
   ```

   ```sql
   -- Find the department with the highest average salary
   -- Tables: employees(emp_id, dept_id, salary), departments(dept_id, name)
   ```

5. **Top N Records**
   ```sql
   -- Find top 5 customers with highest total order amounts
   -- Tables: orders(order_id, customer_id, order_amount)
   ```

   ```sql
   -- Find top 5 selling products in last 3 months
   -- Tables: sales(sale_id, product_id, sale_date, quantity)
   ```

#### Advanced SQL Questions

1. **Window Functions**
   ```sql
   -- Use RANK() to rank employees by salary within each department
   -- Tables: employees(emp_id, dept_id, salary)
   ```

   ```sql
   -- What's the difference between RANK(), DENSE_RANK(), and ROW_NUMBER()?
   -- Write a query demonstrating the difference
   ```

   ```sql
   -- Use LAG/LEAD to compare current month's sales with previous month
   -- Table: monthly_sales(month, sales_amount)
   ```

2. **Duplicate Handling**
   ```sql
   -- Write a query to find duplicate records
   ```

   ```sql
   -- Write a query to delete duplicate records keeping only one copy
   -- Using CTE (Common Table Expression)
   ```

3. **Correlated Subqueries**
   ```sql
   -- Find employees who earn more than their department's average salary
   -- Table: employees(emp_id, dept_id, salary)
   ```

4. **Complex Aggregations**
   ```sql
   -- Find departments where average salary is less than half of the highest salary in the company
   SELECT Department, AVG(Salary) AS AverageSalary
   FROM (
     SELECT Department, Salary
     FROM Employees
     WHERE Salary <= (SELECT MAX(Salary) FROM Employees) / 2
   ) AS Subquery
   GROUP BY Department;
   ```

5. **Query Performance**
   - "How would you optimize this query?
     ```sql
     SELECT *
     FROM orders o
     JOIN customers c ON o.customer_id = c.customer_id
     WHERE o.order_date >= '2024-01-01'
     AND o.status = 'completed'
     AND c.country = 'USA';
     ```
   "
   - "What will you do if your query is running slow?"
   - "How would you handle a query with 300+ lines that's not giving expected output?"

6. **Conditional Aggregation**
   ```sql
   -- Write a query to count number of employees in each department 
   -- who joined in 2024, with and without GROUP BY
   ```

7. **Status Updates**
   ```sql
   -- Write a query to update the status of orders 
   -- based on their delivery dates and print the results
   ```

8. **Date-Based Queries**
   ```sql
   -- Find all orders from the last 3 months
   -- Handle rouge dates in the data
   ```

9. **Common Table Expressions (CTE)**
   ```sql
   -- Rewrite this subquery using CTE:
   SELECT dept_name, 
          (SELECT COUNT(*) 
           FROM employees e 
           WHERE e.dept_id = d.dept_id) as emp_count
   FROM departments d;
   ```

10. **Query Optimization Questions**
    - "How do you tune SQL query performance?"
    - "What factors affect SQL query performance?"
    - "Explain the role of indexes in query optimization."
    - "How do you identify bottlenecks in SQL queries?"

11. **Transaction Management**
    - "What are ACID properties?"
    - "How do you handle transaction deadlocks?"

12. **NULL Handling**
    ```sql
    -- Write a query to handle null values in salary calculation
    -- Show different approaches to handle nulls
    ```

13. **Data Cleaning Queries**
    - "How do you handle duplicate values?"
    - "Write queries to clean and standardize data"
    - "How do you handle NULL values in your queries?"





