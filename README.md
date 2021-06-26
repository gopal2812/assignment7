# Assignment7

TOPIC: Scopes & Closures

ASSIGNMENT
1. Write a closure that takes a function and then check whether the function passed has a docstring with more than 50 characters. 50 is stored as a free variable (+ 4 tests)

2. Write a closure that gives you the next Fibonacci number (+ 2 tests)

3. We wrote a closure that counts how many times a function was called. Write a new one that can keep a track of how many times add/mul/div functions were called, and update a global dictionary variable with the counts (+ 6 tests)

4. Modify above such that now we can pass in different dictionary variables to update different dictionaries (+ 6 tests)

Solution:
1] docstring is a closure which counts the length of docstring in the input function

2] FIBONACCI numbers: The Fibonacci sequence is a series of numbers where a number is the addition of the last two numbers, starting with 0, and 1. The Fibonacci Sequence: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55…

fibonacci returns a function which when called returns the next fibonacci number

3]func_counter is a closure which counts the number of times a function is called and stores the count in a global dictionary.

4] func_counter_dict is a closure which counts the number of times a function is called and stores the count in a dictionary.

