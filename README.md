# #2 - Become a Python Function Ninja 

This assignment involves writing some more functions in Python :+1:  

Last assignment aimed to strengthen your basic function writing skills while also learning the concept of typecasting to convert one data type to another. 

This one will take half an hour, but will teach you all cool things about functions. 

## Notes :  For help in finishing this assignment

### Parts of a Function - Quick Recall
```
def printHello(name):
  print "Hello" + name + "!"
  
printHello("Turtle")
```

```
def add(x, y):
  sum = x+y
  return sum
  
result = add(a, b)
```

- Function Definiton - A header line which begins with a keyword and ends with a colon. 
- Function Declaration - A body consisting of one or more Python statements, each line should be indented the same amount.
- Function call - Defining and Declating a new function does not make the function run. To do that we need a function call. 
- Parameters 
  - These are of two types
    - Formal Parameters - The parameters/variables in the function definition are more specifically known as the formal parameters.
      Eg. def add(x, y):  Here x and y are formal parameters.
    - Actual Parameters - A function needs certain information to do its work. These values, often called arguments or actual parameters, are passed to the function by the user. They are in the function call, eg add(a,b) , a and b are actual parameters
- Return statement 
  -  A function may or may not return anything
  -  A function that does our work but not returns anything, like this one,
      ```
      def printHello(name):
        print "Hello" + name + "!"
  
      printHello("Turtle")
      ```
    are called *procedures* or non - fruitful functions
  -  On the other hand, if it returns something, like
      ```
      def add(x, y):
         sum = x+y
         return sum
  
      result = add(a, b)
      ```
    then the function is called a fruitful function
    
  - The return statement is followed by an expression which is evaluated. Its result is returned to the caller.  Okay sweet! 
    ```
    return a + b 
    ```
    a + b is an expression

### Inside Functions

- Two types of Functions 
  - User-defined, which users write.
  - Built - in functions, example - print(), abs(), len() Okay!
  
- Local Scope and Global Scope [dude this is *important* :smile: ]
  1.  In-Depth Knowledge about variables and data types in Python : [Read](http://www.python-course.eu/python3_variables.php)
  2.  Then this one : [Read](http://www.python-course.eu/python3_global_vs_local_variables.php)
  3.  These two articles are excellent and cover almost every intricate detail and tricks. 
  4.  These articles may take an hour or two to study, but it'll be totally worth it. 
- Remember if you want to know what a built-in function does, just type help(function_name) in Python interpreter
  Eg - help(print)
    help(id)
    help(len)
    help(abs)
    

## Questions

1. Write a function which returns max of 2 numbers. We can use if, elif and else, right?
2.  Find the output - Concept of local and global variables
```
a = 60
def func(z):
    print("z = ", z)
    a = 2
    print('Changed local a to', a)
func(a)
print('Global a is still', a)
```
3. What  is the use of id(), print() function in python? You know the interpreter trick!
4. What's the output: 

```
def cube(x):
    return x * x * x   
 
x = cube(3)    
print x
```
5. Lets find the output , again! :smiley:
```
def foo(k):
    k[0] = 1
q = [0]
foo(q)
print(q)
```
6. Try this, find output?
```
def foo(i, x=[]):
    x.append(x.append(i))
    return x
for i in range(3):
    y = foo(i)
print(y)
```

- The trick for solving 'find the output' questions is to NOT think how the program wants to you to think.  DON'T proceed with any notion of how that program is *supposed* to work, find out how that program will *exactly* work. 

- Try doing dry run! Okay! :smile:
