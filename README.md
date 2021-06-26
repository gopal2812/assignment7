# Assignment7
EpiAssignment

TOPIC: Scopes & Closures

ASSIGNMENT
1. Write a closure that takes a function and then check whether the function passed has a docstring with more than 50 characters. 50 is stored as a free variable (+ 4 tests)

2. Write a closure that gives you the next Fibonacci number (+ 2 tests)

3. We wrote a closure that counts how many times a function was called. Write a new one that can keep a track of how many times add/mul/div functions were called, and update a global dictionary variable with the counts (+ 6 tests)

4. Modify above such that now we can pass in different dictionary variables to update different dictionaries (+ 6 tests)

Solution:
1] docstring is a closure which counts the length of docstring in the input function

def check_doc_string_len(fn):
    """ This a closure which counts the length of the docstring"""
    free_var_local_count = 50
    def check_doc_string_len_inner():
        ''' This function counts the characters in 'fn':function and prints relavent message.
        INPUT: fn : Function
        OUTPUT: RELEVANT message regarding the length of docstring
        '''
        if not isfunction(fn):
            raise TypeError("Inappropriate INPUT:please send in a function")
        nonlocal free_var_local_count
        if len(fn.__doc__) >= free_var_local_count:
            return True
        else:
            return False
    return check_doc_string_len_inner

