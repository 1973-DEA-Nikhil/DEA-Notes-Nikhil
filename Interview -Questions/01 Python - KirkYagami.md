### PYTHON INTERVIEW QUESTIONS

#### Basic Python Questions

1. **Data Types & Collections**
   - "What are the different data types in Python?"
   - "Explain the difference between list and tuple with examples."
   - "Why would you choose a tuple over a list?"
   - "What's the main difference between list and array in Python?"
   - "How do you remove duplicate elements from a list? Write a code example."

2. **String Manipulation**
   ```python
   # Write a program to reverse a string
   # Input: "Hello World"
   # Output: "dlroW olleH"
   ```
   
   ```python
   # Write a program to swap first name and last name
   # Input: "John Doe"
   # Output: "Doe John"
   ```

3. **List Operations**
   ```python
   # Write a program to find the highest element in a list
   # Input: [23, 45, 67, 12, 89, 34]
   # Output: 89
   ```
   
   ```python
   # Write a program to count duplicate elements in a list
   # Input: [1, 2, 2, 3, 4, 4, 5]
   # Output: {2: 2, 4: 2}
   ```

4. **Lambda Functions**
   ```python
   # What would be the output of this code?
   x = [1, 2, 3, 4]
   li = [lambda x: x**2]
   print(li)
   # Explain why this outputs what it does
   ```

5. **Problem Solving**
   ```python
   # Write a function to check if a string is palindrome
   def is_palindrome(s):
       # Write your code here
       pass
   
   # Test cases
   # "radar" -> True
   # "hello" -> False
   ```

#### Advanced Python Questions

1. **Exception Handling**
   ```python
   # What would be the output of this code?
   def divide_numbers(a, b):
       try:
           result = a / b
           print("Division result:", result)
       except ZeroDivisionError as e:
           print("Error:", e)
       except TypeError as e:
           print("Error:", e)
       else:
           print("No exception occurred.")
       finally:
           print("This block always executes.")

   # Test cases:
   divide_numbers(10, 2)
   divide_numbers(10, 0)
   divide_numbers("10", 2)
   ```

2. **Decorators**
   - "What are decorators in Python? Provide an example."
   - "How would you create a decorator to measure the execution time of a function?"
   ```python
   # Write a decorator that prints function execution time
   ```

3. **OOP Concepts**
   ```python
   # Write a class with constructor and demonstrate inheritance
   class Employee:
       # Write your code here
       pass
   
   class Manager(Employee):
       # Write your code here
       pass
   ```
   - "What is the purpose of 'self' in Python classes?"
   - "Explain method overriding with an example."

4. **Memory Management**
   - "How does garbage collection work in Python?"
   - "What are reference cycles?"
   - "Explain memory management in Python."

5. **Performance Optimization**
   ```python
   # How would you optimize this code?
   def find_element(lst, target):
       for i in range(len(lst)):
           if lst[i] == target:
               return True
       return False
   ```
   - "How can you improve the performance of Python code?"
   - "What are the best practices for writing optimized Python code?"

6. **Multithreading**
   - "What is the difference between multiprocessing and multithreading in Python?"
   - "How would you implement a thread-safe counter in Python?"
   ```python
   # Write a simple multithreaded program
   ```

7. **Generators**
   - "What are generators in Python? How are they different from regular functions?"
   - "Write a generator function that yields fibonacci numbers."

8. **Scenario-Based Questions**
   ```python
   # You have a large dataset and need to process it efficiently.
   # How would you implement this using Python?
   # Consider memory constraints and performance.
   ```

9. **Code Review Questions**
   ```python
   # What's wrong with this code and how would you improve it?
   def process_list(lst):
       new_lst = []
       for i in range(len(lst)):
           new_lst.append(lst[i] * 2)
       return new_lst
   ```

10. **Debug Questions**
    ```python
    # This code has a bug. Find and fix it.
    def merge_dicts(dict1, dict2):
        dict1.update(dict2)
        return dict1
    
    # Test case
    d1 = {'a': 1}
    d2 = {'b': 2}
    result1 = merge_dicts(d1, d2)
    result2 = merge_dicts(d1, {'c': 3})
    print(d1)  # What's the issue here?
    ```
