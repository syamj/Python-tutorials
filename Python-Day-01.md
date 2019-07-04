
# Python

- Python is a general-purpose interpreted, interactive, object-oriented, and high-level programming language. It was created by Guido van Rossum during 1985- 1990.
- Like Perl, Python source code is also available under the GNU General Public License (GPL).


# Variable types in Python

Below are different types of variables in Python.

```hl-ipython3
- int
- float
- string
- list
- dictionary
- tuple
```


# Integer Declaration (int)


```python
#Integer values can be assigned directly using ''=''

age = 10
```


```python
print(age) #Print function is used to print the value of a variable.
```

    10



```python
type(age) #We can find out the datatype of a variable using type() function
```




    int




```python
age #We use Jupyter-notebook to write this tutorial, here just entering a variable will print it's value.
```




    10



# Float Declaration (float)


```python
#Any value which contains a decimal point is considered as a float variable.

price = 10.64
```


```python
price
```




    10.64




```python
type(price)
```




    float




```python
#Float cannot recognize any variables with more than one '.'

ip = 10.0.0.1
```


      File "<ipython-input-11-3bf74e90f524>", line 3
        ip = 10.0.0.1
                  ^
    SyntaxError: invalid syntax



# String Declaration (str)


```python
#A string should be declared inside a '' or ""

name = 'syam'
```


```python
type(name)
```




    str




```python
#Any numbers or alphabets can be saved as a string.

ip = '10.0.0.1'
```


```python
type(ip)
```




    str




```python
#Even numbers enclosed in '' or "" will be considered as a string.

age = '31'
```


```python
type(age)
```




    str



# Basic Mathematical Operations using Python


```python
x = 10
y = 3
```


```python
#Addition

x + y
```




    13




```python
#Subtraction

x - y
```




    7




```python
#Multiplication

x * y
```




    30




```python
#Division

x / y
```




    3.3333333333333335




```python
#Floor Division - Here the values of variables will be divided but returns only a whole number value.

x // y
```




    3




```python
#Modulus - Divides and returns the remainder.

x % y
```




    1



> All the above operations can only be done on an integer.


```python
price = '10' #Here 10 is a string
quantity = 5 #Here 5 is an integer
```


```python
#When a string is multiplied by int, below happens.
price * quantity 
```




    '1010101010'




```python
#Another example

'a' * 20
```




    'aaaaaaaaaaaaaaaaaaaa'



# Converting a string into Integer


```python
x = '10' #A string is declared
```


```python
y = int(x) #int() will convert string to integer. Here value of y will be integer 10 and value of x will remain str
```


```python
y
```




    10




```python
type(y)
```




    int




```python
x * 5 #Since x is still str, it return below value
```




    '1010101010'




```python
int(x) * 5 #x is converted to int and then multiplied with 5
```




    50



# Length function


```python
#Len() is used to find the length of a string.

lang = 'malayalam'
len(lang)
```




    9




```python
#We cannot calculate the length of an integer

atm_pin = 1234
len(atm_pin)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-41-2edc3670c39b> in <module>
          1 atm_pin = 1234
    ----> 2 len(atm_pin)
    

    TypeError: object of type 'int' has no len()


# Converting to string 


```python
str(atm_pin) #str() can be used to convert integer to string.
```




    '1234'




```python
len(str(atm_pin)) #So we can now calculate the length of an integer
```




    4



# Comparison Operators


```python
10 > 5 #Here the output will be boolean (True or False)
```




    True




```python
5 < 5
```




    False




```python
5 < 5 or 5 == 5 #if any one of o/p is True, or returns True. == is used to compare if values are equal.
```




    True




```python
1 <= 1
```




    True



# String Membership Operation


```python
fruit = 'pineapple'
```


```python
'apple' in fruit #This will return True because while traversing through pineapple and check for the string apple in it.
```




    True




```python
'app' not in fruit #This statement is False because string app is present in pineapple
```




    False




```python
'syam' not in fruit #This statement is True because string syam is not present in pineapple
```




    True



# Input() Function


```python
#This function is used to read values from keyboard input.

input()
```

    Syam





    'Syam'




```python
name = input("Please enter your name: ") #This will print the message and wait for your keyboard input.
```

    Please enter your name: Syam



```python
pin = input("Please neter your ATM PIN: ")
```

    Please neter your ATM PIN: 1234



```python
type(pin) #All input read via input() will be considered as a string.
```




    str



# If condition


```python
#If condition is used to check if a statement is tru or false and execute certain commands respectively.

original = 4556
pin = input("Please Enter your ATM PIN : ")

if int(pin) == original:                   #Checking if entered pin is equal to value set to variable 'original'
  print("Success")                         #If True it will execute this
  print("Dummy Message")                   #And this and any other line coming with same indentation
else:                                      #If entered pin is not equal, it will execute the commands below this line
  print("Failed")
```

    Please Enter your ATM PIN : 1234
    Failed


# String Methods


```python
lang = 'Malayalam'
```


```python
id(lang) #Every string will be assigned a unique id which will be modified when the value of variable changes,
```




    139638595136688




```python
lang = 'English'
id(lang)
```




    139638595162720



# dir()


```python
#dir() any value will print whatever default modules can be used to it.

dir(lang)
```




    ['__add__',
     '__class__',
     '__contains__',
     '__delattr__',
     '__dir__',
     '__doc__',
     '__eq__',
     '__format__',
     '__ge__',
     '__getattribute__',
     '__getitem__',
     '__getnewargs__',
     '__gt__',
     '__hash__',
     '__init__',
     '__init_subclass__',
     '__iter__',
     '__le__',
     '__len__',
     '__lt__',
     '__mod__',
     '__mul__',
     '__ne__',
     '__new__',
     '__reduce__',
     '__reduce_ex__',
     '__repr__',
     '__rmod__',
     '__rmul__',
     '__setattr__',
     '__sizeof__',
     '__str__',
     '__subclasshook__',
     'capitalize',
     'casefold',
     'center',
     'count',
     'encode',
     'endswith',
     'expandtabs',
     'find',
     'format',
     'format_map',
     'index',
     'isalnum',
     'isalpha',
     'isdecimal',
     'isdigit',
     'isidentifier',
     'islower',
     'isnumeric',
     'isprintable',
     'isspace',
     'istitle',
     'isupper',
     'join',
     'ljust',
     'lower',
     'lstrip',
     'maketrans',
     'partition',
     'replace',
     'rfind',
     'rindex',
     'rjust',
     'rpartition',
     'rsplit',
     'rstrip',
     'split',
     'splitlines',
     'startswith',
     'strip',
     'swapcase',
     'title',
     'translate',
     'upper',
     'zfill']



> We can use any of the above modules to modify the output of value lang.


## Upper()


```python
lang.upper() #This will traverse through the string and change it's values to UPPER CASE.
```




    'ENGLISH'



## lower()


```python
lang.lower() #This will traverse through the string and change it's value to LOWER CASE.
```




    'english'



## count()


```python
lang = 'MalAyalAM' 
```


```python
lang.count('a') #This will count only 'a' in the above variable 'A' will not be considered.
```




    2




```python
#So to check the correct number of 'a' we need to convert to upper or lower.
lang.lower().count('a')
```




    4



## replace()


```python
lang.replace('a','x') #This will replace all 'a' with 'x' (Note : 'A' will not be considered here also)
```




    'MxlAyxlAM'




```python
str.replace? #Adding a ? after any inbuilt function will provide info about it.
```

## endswith()


```python
#To check if a string ends with a specific value. It will return a boolean value.

conf = '/etc/httpd/conf/httpd.conf'
conf.endswith('.conf')
```




    True



## startswith()


```python
#To check if a string starts with a specific value. It will also return a boolean value.

conf.startswith('/etc')
```




    True



## isdigit()


```python
#To check if a string is a digit or not.

number = '12345'
number.isdigit()
```




    True




```python
#If it contains any alphabets, it will return False

number='123gcv' 
number.isdigit()
```




    False



## isalpha()


```python
#To check if a string contains only alphabets

name = 'syam'
name.isalpha()
```




    True




```python
conf = '/etc/httpd/conf/httpd.conf'
conf.isalpha()
```




    False



## rstrip()


```python
#To remove any values from the right side of a string. 
#If no arguements are given, white spaces will be removed.

name = '   syam   '
name.rstrip()
```




    '   syam'




```python
name.rstrip('am   ')
```




    '   sy'



## lstrip()


```python
#To remove any values from left side of a string.
#If no arguements are given, white spaces will be removed.

name.lstrip()
```




    'syam   '



## strip()


```python
#This will search for occurances of a string and remove it from left and right end.
#If no arguements are given, white spaces will be removed.
name.strip()
```




    'syam'




```python
name.strip('   s')
```




    'yam'




```python
name = '-------syam--'
name.strip('-')
```




    'syam'




```python
name = '<color><h1>'
name.strip('<').strip('>')
```




    'color><h1'



# String Indexing


```python
#The characters in a string is indexed and can be accessed using an index number.
#By default index number starts with 0.

name = 'syam' 
name[0]
```




    's'




```python
#We can read the string from backwards as well using '-'

name[-1]
```




    'm'




```python
name[-2]
```




    'a'



# String Slicing


```python
timestamp = '12/Dec/2015:18:25:11'
```


```python
#We can slice a string using indexes.

timestamp[0:11]           #Here it will print from index 0 - 10.
```




    '12/Dec/2015'




```python
#The same can be done like this also.

timestamp[:11] 
```




    '12/Dec/2015'




```python
#This can also be reversed.

timestamp[12:]         #This will print from the 12th index to the end of string.
```




    '18:25:11'




```python

```
