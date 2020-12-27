# **Python Fundamentals**
### **Basic Output**
`print("Hello World")`  
*output : Hello World*  
syntax : `print(*objectsv, sep='' , end='' , file='' , flush=)`  
* Objects : Variables ; if you want to write just a text , you can write your text inside " ".
* sep : You can define the character print between objects. Default value = ' '
* end : You can define the character print end of the last object. Default value = '\n'. This means new line.
* file : You can define the file you want to print objects inside it.
* flush : Flush is used to flush (clear) the internal buffer/stream (or we can say it is used to flush the output stream), it has two values "False" and "True". This description is kind of complex , you can understand with an example  

*example1 :*  
`from time import sleep`  
`print("Hello", end=' ' , flush=False)`  
`sleep(5)`  
`print("World")`  
#output : Hello was printed and World was printed after that without waiting  

*example2 :*  
`from time import sleep`  
`print("Hello", end=' ' , flush=True)`  
`sleep(5)`  
`print("World")`  
#output : Hello was printed and World was printed after 5 seconds
### **Python Variables**
`x = 1`  
This is a python variable. Variables keep its Values. value could be a number , a string , a character , a list...  

*examples :*  

`x = 1.5`  
`y = "Hello World"`  
`a , b , c = 10 , 20 , " Hi"`   
`values : a = 10 , b = 20 , c = "Hi"`  
`d = e = f = 10`  
`values : d = 10 , e = 10 , f = 10`  
`fruits = ["apple", "banana", "cherry"] #list`  
`numbers = (1, 2, 3) #tuple`  
`alphabets = {'a':'anything', 'b':'big', 'c':'curious'} #dictionary`  
`vowels = {'a', 'e', 'i' , 'o', 'u'} #set`  

**Multi-Line Statement**  
You can create multi-line statements with () , [] , {}  
`i = 1 + 2 + 3 + \`  
    `4 + 5 + 6 + \`  
    `7 + 8 + 9`  

`i = (1 + 2 + 3 + `  
    `4 + 5 + 6 + `  
    `7 + 8 + 9)`

`colors = ['red',`   
          `'blue',`  
          `'green']`

`j = 100 ; f = 200 ; k = 300`  

### **Comments**
`# this is a one line comment`  
`"""`  
`this`  
`is `  
`multi-line`  
`comment`  
`"""`  
### **Python Data Types**
type() function shows data type
example:  
`x = 1;print(type(x))`  
#output : <class 'int'>  
isinstance() funcstion returns True if object in  class.  
example:   
`print(isinstance(x,int))`  
#output : True  
#### **Numbers**

* integer = 1
* float = 1.1
* complex = 1+1j
* binary = 0b10110
* octal = 0o476
* hexadecimal = 0xF

#### **Lists**
Lists are collections of multiple variables. You can change the list you created , you can add or delete new items.  
list1 = ["hello world",1,1.5]

#### **Tuples**
Tuples are collections like lists but you can't change tuples. They are close to edit.  
tuple1 = ("hello world",1,1.5)

#### **Sets**
Sets are unordered collections. Sets don't include same members.    
`set1 = {1,2,2,3,3,3}`  
`print(a)`  
#output : {1,2,3}


#### **Dictionaries**
Dictionaries are collections that have key and value.  
 dict1 = {"key1":"value1","key2":"value1"}

*I will write a detailed text about **lists** , **tuples** , **sets** and **dictionaries**.*

#### **Strings**
Strings are collections of characters that inside of " ".  
"Hello World"

#### Type Conversations
* float(5) = 5.0
* int(5.6) = 5
* int("5") = 5
* str(5) = '5'
* set([1,2,3,4,5]) = {1,2,3,4,5}
* list((1,2,3,4,5)) = [1,2,3,4,5]
* list("12345") = ["1","2","3","4","5"]
* tuple([1,2,3,4,5]) = (1,2,3,4,5)
* dict([1,2],[3,4],[5,' ']) = {1:2,3:4,5:''}


### **Getting User Input**  
*variable* = input(*input message*)  
example:
```
x = input("What is your name? : ")
print(f"Hello {x}")
```

### **Importing Modules**
```
import math
print(math.pi)
```
```
from math import pi
print(pi)
```
```
import math as m
print(m.pi)
```
```
from math import pi as PI
print(PI)
```
Also you can import your python module/file.
if you have a file in another file , you can add it to default modules directory.
```
import sys
sys.path.append(../moduledir)
import module
```
In this example , you can import module module in moduledir directory of parent directory.

### **Operators**  

#### *Arithmetic Operators*
* '+' : summary
* '-' : subtraction
* '*' : multiplication
* '/' : division
* '%' : modulus
* '//' : floor division
* '**' : exponent  

#### *Comparsion Operators*
* '>' : grater than
* '<' : smaller than
* '==' : equal to
* '>=' : grater than or equal to
* '<=' : smaller than or equal to
* '!=' : not equal to

#### *Logical Operators*
* 'and' = Logical and
* 'or' = Logical or
* 'not' = Logical not

#### *Bitwise Operators*
* '&' : Bitwise and
* '|' : Bitwise or
* '~' : Bitwise not
* '^' : Bitwise xor
* '>>': Bitwise right shift
* '<<': Bitwise left shift

#### *Assignment Operators*
* '='
* '+='
* '-='
* '*='
* '/='
* '%='
* '//='
* '**='
* '&='
* '|='
* '~='
* '^='
* '>>='
* '<<='

example:
```
x = 10
x **= 2
print(x)
#output = 100
* x = x ** 2
```

#### *Identity and Membership Operators*
* is = True if the operands are identical
* is not = True if the operands are not identical
* in = True if value/variable is found in the sequence
* not in = True if value/variable is not found in the sequence

### **Conditions**
```
if test statement:  
    <commands>
elif secondary test statement:
    <commands>
<other elif statements as much as you want>
else :
    <commands that will work if any if statement doesn't work>
```
**Don't forget , tab is very important.**
### **Loops**
```
while statement:
    <commands>
#this will work if statement don't be false.
for i in list:
    <command>
#everything that you did with i will do
#for all elements of list.
```
#### **Break , Continue and Pass**
* break ends loops
* continue skips commands under of it in a loop
* Pass is a placeholder for empty statements

### **Functions / Methods**
A function do a specific task.
Syntax:
```
def function_name(parameters):
	"""docstring"""
	<commands>
```
example:
```
def sayHello(str):
    """
    Just says hello to str
    """
    print(f"Hello {str}")

sayHello("Nicola")
```
and You can access docstring of function like this.
`print(sayHello.__doc__)`

Functions can return anything
```
def square(x):
    """
    returns x**2
    """
    return x**2
```
You can work with no numbered arguments.
```
def summary(*numbers):
    x = 0
    for i in numbers:
        x += i
    return x
print(summary(1,2,3,4,5))
```
#### **Recursion**
If a function calls itself , it is a recursive function.
```
def fib(int):
    if int <= 0:
        return f"error , {int} is not an option."
    elif int == 1:
        return 1
    elif int == 2:
        return 1
    else :
        return fib(int-1)+fib(int-2)
```
#### **Lambda Functions**
Syntax:
`lambda argument : statement`
example:
```
cube = lambda x : x**3
print(cube(3))
```

### **Lists**
* **list** = [0,1,2]
* **list[0]** = 0
* **list[0:2]**








 = 0,1
* **list.append(*member*)** : adding a member to end of the list.
* **list.insert(*index*,*member*)** : adding a member to index of list
* **list.extend(*another list*)** : appending members to list from another list
* **list.remove(*member*)** : deleting first member element of list
* **list.pop(*index*)** : returns element of index. if you don't enter a parameter , returns the  last element.
* **list.index(*member*)** : returns the first member  element
* **list.sort()** : sets indexes of members alphabetically
* **list.revers()** : sets indexed of members revers.
* **list.count(*member*)** : returns there is how many member elements in the list.
***

Websites i used :  
* [Programiz](https://www.programiz.com/)
