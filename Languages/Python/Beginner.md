# **Basic I/O**
## _Basic Output_
_print("Hello World")_  
_output : Hello World_  
syntax : print(*objectsv, sep='' , end='' , file='' , flush=)  
* Objects : Variables ; if you want to write just a text , you can write your text inside " ".
* sep : You can define the character print between objects. Default value = ' '
* end : You can define the character print end of the last object. Default value = '\n'. This means new line.
* file : You can define the file you want to print objects inside it.
* flush : Flush is used to flush (clear) the internal buffer/stream (or we can say it is used to flush the output stream), it has two values "False" and "True". This description is kind of complex , you can understand with an example  

_example1 :_  
```
from time import sleep  
print("Hello", end=' ' , flush=False)  
sleep(5)  
print("World")  
#output : Hello was printed and World was printed after that without waiting
```

_example2 :_  
```
from time import sleep  
print("Hello", end=' ' , flush=True)  
sleep(5)  
print("World")  
#output : Hello was printed and World was printed after 5 seconds
```
## _Basic Input_  
*variable* = input(*input message*)  
example:
```
x = input("What is your name? : ")
print(f"Hello {x}")
```
***
# **Variables and Data Types**
type() function shows data type
example:  
```
x = 1;print(type(x))  
#output : <class 'int'>
```   
isinstance() funcstion returns True if object in  class.  
example:   
```
print(isinstance(x,int))  
#output : True
```
## **Numbers**

* integer = 1
* float = 1.1
* complex = 1+1j
* binary = 0b10110
* octal = 0o476
* hexadecimal = 0xF

## **Lists**
Lists are collections of multiple variables. You can change the list you created , you can add or delete new items.  
list1 = ["hello world",1,1.5]

## **Tuples**
Tuples are collections like lists but you can't change tuples. They are close to edit.  
tuple1 = ("hello world",1,1.5)

## **Sets**
Sets are unordered collections. Sets don't include same members.    
```
set1 = {1,2,2,3,3,3}  
print(a)  
#output : {1,2,3}
```
## **Dictionaries**
Dictionaries are collections that have key and value.  
 dict1 = {"key1":"value1","key2":"value1"}

*I will write a detailed text about **lists** , **tuples** , **sets** and **dictionaries**.*

## **Strings**
Strings are collections of characters that inside of " ".  
"Hello World"

## Type Conversations
* float(5) = 5.0
* int(5.6) = 5
* int("5") = 5
* str(5) = '5'
* set([1,2,3,4,5]) = {1,2,3,4,5}
* list((1,2,3,4,5)) = [1,2,3,4,5]
* list("12345") = ["1","2","3","4","5"]
* tuple([1,2,3,4,5]) = (1,2,3,4,5)
* dict([1,2],[3,4],[5,' ']) = {1:2,3:4,5:''}  

***

# **Operators**  

## *Arithmetic Operators*
* '+' : summary
* '-' : subtraction
* '*' : multiplication
* '/' : division
* '%' : modulus
* '//' : floor division
* '**' : exponent  

## *Comparsion Operators*
* '>' : grater than
* '<' : smaller than
* '==' : equal to
* '>=' : grater than or equal to
* '<=' : smaller than or equal to
* '!=' : not equal to

## *Logical Operators*
* 'and' = Logical and
* 'or' = Logical or
* 'not' = Logical not

## *Bitwise Operators*
* '&' : Bitwise and
* '|' : Bitwise or
* '~' : Bitwise not
* '^' : Bitwise xor
* '>>': Bitwise right shift
* '<<': Bitwise left shift

## *Assignment Operators*
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
#x = x ** 2
```

## *Identity and Membership Operators*
* is = True if the operands are identical
* is not = True if the operands are not identical
* in = True if value/variable is found in the sequence
* not in = True if value/variable is not found in the sequence

***

# **Comments**
```
#this is one line comment
"""
this is
multiple
lines
comment
"""
```

***

# **Conditions**
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

***

# **Loops**
```
while statement:
    <commands>
#this will work if statement don't be false.
for i in list:
    <command>
#everything that you did with i will do
#for all elements of list.
```
**Tabs are important again**
## **Break , Continue and Pass**
* break ends loops
* continue skips commands under of it in a loop
* Pass is a placeholder for empty statements

***

# **Iterables**

## **Lists**
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
* **del list** : deletes list

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
_Membership tests are done in keys ,  iterating through is done in values_


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
_if you make a variable as str , you can get an error , these are placeholder._

***

# **Importing Modules**
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

# **Functions**
```
def func(parameter):
    codes

func(parameter) # calling function
```
example:
```
def sum(num1 , num2):
    return num1 + num2
```
**return** is value of function.

WE can create default arguments:
```
def sum(num1 = 0 , num2 = 0):
    return num1 + num2
```
You can define function for limitless arguments like this.
```
def sum(*nums):
    result = 0
    for i in nums:
        result += i
    return result
print(sum(1,2,3,4,5,6,7,8,9))
```
and you can define it with keyword arguments
```
def sum(**nums):
    result = 0
    for i in nums:
        result += i
    return result
print(sum(num1=1,num1=2))
```
## **Specials Parameters**
you can give permission for parameter usage like this
def func(positional_parameters,/,pst_or_kwd_parameters,*,kwd parameters)
example :
```
def sum(num1,num2,/):
    return num1 + num2
```
if you call the function like this sum(num1=1,num2=2) , you will get error

## **Unpacking**
```
def sum(*args):
    result = 0
    for i in args:
        result += i
    return result
numbers = [1,2,3,4,5,6,7,8,9]
```
If you write sum(numbers) , you will get error. You have to write sum(*numbers). If you want to do same thing with a dictioary , you have to use double asteriks symbol.

## **Lambda Expressions**
```
name = lambda arguments : expression
```

example:
```
sum = lambda a,b : a+b
print(sum(10,20))

```
## **Annotations**
```
def func(parameter:'annotations'=default-value):
    
```
Annotation is a definion about parameters.
example:
```
def sum(num1 : int = 0 , num2 : int = 0):
    return num1 + num2
print(sum.__annotations__)
#output
#Annotations : {'num1' : <class 'int'>,'num2' : <class 'int'>}
```
## **Function Docstrings**
```
def func(parameters):
    """
    definion about function
    """
```
This is a definion about function.
example:
```
def sum(*args=0,):
    """
    Returns summary of numbers that you gave as parameters. If you
    don't give any parameters , that returns 0
    """
    result = 0
    for i in args:
        result += i
    return result
print(sum.__doc__)
```
# **File Handling**
variable = open('filename','mode')
## **File methods**
f.read() : reads entire file , returns string
f.readline() : reads lines one-by-one at everytime you call the function , returns string
f.readlines() : reads lines appends every line to a list and returns list.
f.write(str) : writes str to file
f.writelines(list) : writes list to lines in file
