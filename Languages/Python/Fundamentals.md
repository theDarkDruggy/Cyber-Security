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
