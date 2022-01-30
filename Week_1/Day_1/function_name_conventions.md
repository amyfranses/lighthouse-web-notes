# Function Naming Conventions

1 - Give your functions verb/action based names.

2 - Use camelCasedNames

3 - Properly indent the function code.

4 - Functions should focus on a single task:    returning a value or causing a side effect. 
       
       - Break your function into additional smaller functions if you find it doing two or more things
           
           - One single task could be to compute and return a value.
           
           - Another single task could be to perform a side effect such as logging a message to the screen
            
5 -  It is ideal if functions try to avoid reading outer scope variables. 
If a function needs some information / data, then that **data should instead be passed in as a parameter,** making it available within the **function's inner scope.**
           