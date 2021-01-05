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
* **list[-1]** = 2
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
* del list : deletes list

### **Tuples**
* **tuple** = (1,2,3)
* **tuple** = 1 , 2 , 3
    * a , b , c = tuple
    * a = 1 , b = 2 , c = 3
* **tuple** = (1,) : tuple with one element
* **tuple** = (1,2,3)
* **tuple[0]** = 1
* **tuple[-1]** = 3
* **tuple[0:2]** = (1,2)
* **del tuple**  deletes tuple
* **tuple.count(*member*)** : returns there is how many functions in the tuples
* **tuple.index(*member*)** : returns index of member
### **Sets**
* **set** = {1,2,3}
* **set.add(*element*)** : adds an element
* **set.update(*elements*)** : adding elements that more than online
* **set.discard(*element*)** : delete element , if there is no element , doesn't cause to error
* **set.remove(*element*)** : delete element , if there is no element , causes to error
* **set.pop()** : returns a random elements
* **set.clear()** : deletes all elements
* **set.union(*another set*)** : returns merged situation
* **A | B** : returns merged situation
* **A & B** : returns elements that is element of both
* **A.intersection(B)** : returns elements that is element of both
* **A - B** : returns difference between A and B
* **A.difference(B)** : returns difference
* **A ^ B** : returns (A | B) - (A & B)
* **A.symmetric_difference(B)** : returns (A | B) - (A & B)
### **Dictionaries**
* **dict** = {'a':"apple",'b':"broadcast"}
* **dict['a']** = "apple" #access
* **dict['c']** = "car" #adding
* **dict.pop(a)** : deletes a and returns key
* **dict.clear()** : deletes all elements
* **del dict** : deletes dict
*Membership tests are done in keys ,  iterating through is done in values*


### **Strings**
* **string** = "123"
* **string** = '123'
* **string** = """123"""
* **string** = '''123'''
* **string[0]** = "1"
* **string[-1]** = "3"
* **string[0:2]** = "12"
* **string =**f"text{variable}"
* **str.capitalize()** : returns the situation that first letter is upper case
* **str.upper()** : returns the situation that all of letters is upper case
* **str.lower()** : returns the situation that all of letters is lower case
* **str.swapcase()** : returns the situation that all of letters is another case
* **str.title()** : returns  the situation that  first letters of words is upper case
* **str.center(x)** : leaves blank at right and left x times
* **str.center(x,'#')** : adds # at right and left x times
* **str.ljust(x)** : text get closer to left and leaves blanks at right x times
* **str.ljust(x,"y")**  :  text get closer to left and adds y to right x times
* **str.rjust()**  : totally opposite of ljust
* **str.replace('x','y')**  : turn x into y
* **str.startswith('e')**  : if str starts with e , it returns true
* **str.endswith("e")** : if str ends with e , ir returns true
* **str.count("e")** : returns there is  how many e letters in str
* **str.isalpha()** : returns true if there is only letters in str
* **str.isdigit()** : returns true if there is only numbers in str
* **str.isalnum()** : returns true if there is numbers and letters in str
* **str.islower()** : returns true if all of letters is lower case
* **str.isupper()** : totally opposite of islower()
* **str.istitle()** : returns true if str is title
* **str.isspace()** : returns true if there is only space character
* **str.expandtabs(x)** : turns tabs into x space
* **str.find('a')** : finds and says index in the str
* **str.find("a")** : finds and says index in the str but searches right to left
* **str.join("x")** : adds x between all of characters
* **str.strip()** : deletes characters like space and /n at right and left( there is functions like str.lstrip() and str.rstrip)
*if you make a variable as str , you can get an error , these are placeholder.*
### **File Handling**

Opening file in current directory:  
* f = open("text.txt")
* with open("text.txt") as f

Opening file in another directory:  
* f = open("**dir**/text.txt")
* with open("**dir**/text.txt") as f  

f = open(**file**,**mode**,encoding=)
**Modes**
* r : reading mode
* w : writing mode , if there is no file , it will be created.
* x : exclusive creation
* a : appending mode
* t : text mode ( default )
* b : binary mode
* +: Open file for reading and writing
* r+ : reading and writing
* w+ : writing and reading
* a+ : appending and reading

**Some Other Functions**
**f.close()** : close the file  
**f.read()** : reads all of file as a string  
**f.readlines()** : reads lines as list  
**f.write(*str*)** : writes to file  
**f.writelines(*str*)** : writes  to file every member is one line

### **Exception Handling**
* Syntax Error  
* Logical Errors ( Exception )  

You can catch exceptions and you can block ending of program.
```
x = int(input("enter a number"))
try :
    print(2520 / x)
except:
    print("You entered a wrong number")
finally:
    #you can wwrite last commands here , this is
    #optional
```
You can define your errors
```
# define Python user-defined exceptions
class Error(Exception):
    """Base class for other exceptions"""
    pass


class ValueTooSmallError(Error):
    """Raised when the input value is too small"""
    pass


class ValueTooLargeError(Error):
    """Raised when the input value is too large"""
    pass


# you need to guess this number
number = 10

# user guesses a number until he/she gets it right
while True:
    try:
        i_num = int(input("Enter a number: "))
        if i_num < number:
            raise ValueTooSmallError
        elif i_num > number:
            raise ValueTooLargeError
        break
    except ValueTooSmallError:
        print("This value is too small, try again!")
        print()
    except ValueTooLargeError:
        print("This value is too large, try again!")
        print()

print("Congratulations! You guessed it correctly.")
```
### **OOP**
#### **Defining Class**
```
class worker:
	pass
```
#### **Defining Object**
```
Bob = worker()

```
_Example_
```
class worker:
	#attributes
	salary = 0
	
	#initializer function
	def __init__(self,salary):
		self.salary = salary

	def setsalary(self,salary):
		self.salary = salary
	def getsalary(self):
		return self.salary
Bob = Worker(8500)
Bob.setsalary(7500)
print(Bob.getsalary())
#output : 7500
```
***

Websites i used :  
* [Programiz](https://www.programiz.com/)
