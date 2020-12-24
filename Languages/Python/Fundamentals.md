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
`#output : Hello was printed and World was printed after that without waiting`  

*example2 :*  
`from time import sleep`  
`print("Hello", end=' ' , flush=True)`  
`sleep(5)`  
`print("World")`  
`#output : Hello was printed and World was printed after 5 seconds`
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

***

Websites i used :  
* [Programiz](https://www.programiz.com/)
