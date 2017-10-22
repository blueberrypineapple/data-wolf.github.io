---
layout: post
title: Python for Data Wolves
subtitle: Learn, use and re-use
---
![jpg](https://github.com/data-wolf/data-wolf.github.io/blob/master/img/Optimized-Data_Wolf.jpg?raw=true)
## Python (1991)
The first three reasons to use Python for Data Science: NumPy, Pandas and Jupyter Notebooks. The sheer power of these three libraries alone makes them an invaluable resource for the aspiring data scientist. Python has a healthy eco-system extending it's reach far beyond Numpy, Pandas and Jupyter Notebooks, in fact, the Python community is growing at a swift rate showing no signs of slowing down. MongoDB has PyMongo for example, not to mention Matplotlib, SciPy and many more... Be sure to check out [Python Tutor](http://pythontutor.com) for a great online behind the scenes look at python.

## Variables 
* Numeric: intergers, floats and complex
* Sequence: list, tuples and range
* Binary: byte and byte array
* True/False: bool
* Text:  string


## Objects
Everything in Python is an Object. Objects hold data and can have actions associted with them like lists.

## Loops

### For Loops
Here is a for loop using range. 0 is inclusive and 6 is exclusive, so Python prints 0-5 and not 0-6.


```python
for i in range(0,6):
    print(i)
```

    0
    1
    2
    3
    4
    5


Next we repeat the same loop but we add an argument to(0,6) to (0,6,2).
The 2 means size of count or range, so it will now print every other number.


```python
for i in range(0,6,2):
    print(i)
```

    0
    2
    4



```python
#here we can make range larger and moving in incriments of 5
for i in range(0,100,5):
    print(i)
```

    0
    5
    10
    15
    20
    25
    30
    35
    40
    45
    50
    55
    60
    65
    70
    75
    80
    85
    90
    95


### While Loops


```python
i=0
while i<12:
    print(i)
    i+=1
```

    0
    1
    2
    3
    4
    5
    6
    7
    8
    9
    10
    11


### If


```python
i=3
if i>2:
    print(i)
```

    3


### Else


```python
i=1
if i>2:
    print(i)
else:
    print('Hi.')
```

    Hi.


### If, Elif and Else
First you have an if statement.
Then you have if then else.
Now you can have ***if* ** in front and ** *else* ** at the very end and as 
many ** *elif* ** as you need in the middle(sort of). So the order we have for our demo code is: ** *if, elif, elif, else.* **


```python
i=1
if i>2:
    print('Greater than two.')
elif i<2:
    print('Less than two.')
else:
    print("It's 2!")
```

    Less than two.



```python
i=2
if i>2:
    print('Greater than two.')
elif i<2:
    print('Less than two.')
else:
    print("It's 2!")
```

    It's 2!



```python
i=3
if i>2:
    print('Greater than two.')
elif i<2:
    print('Less than two.')
else:
    print("It's 2!")
```

    Greater than two.


## Functions
Define, name and input variables if any.
Add conditions for the Function to run when called.


```python
def x_plus_y(x,y):
    print(x+y)

```


```python
#When we call x_plus_y we need to enter two intergers. ie. 2,5
x_plus_y(2,5)
```

    7



```python
x_plus_y(333,-872.4)

```

    -539.4



```python
#You can trick python and add strings because x=? both or a float.
x_plus_y('You super ','freak dancer!')
```

    You super freak dancer!



```python
#You can't however mix :(
x_plus_y("you",872)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-86-30edba64e9c7> in <module>()
          1 #You can't however mix :(
    ----> 2 x_plus_y("you",872)
    

    <ipython-input-82-426d83101ffd> in x_plus_y(x, y)
          1 def x_plus_y(x,y):
    ----> 2     print(x+y)
    

    TypeError: must be str, not int


### See how cool python is!
It just tells you. You can learn much from errors, stay crispy.
#### TypeError: must be str, not int

# Basic String Operatioms

## Change case


```python
word = "absquatulate"
word.upper()
```




    'ABSQUATULATE'




```python
word
```




    'absquatulate'



### In reverse order
Using .lower()



```python
word = "ABSQUATULATE"
word.lower()
```




    'absquatulate'



## Concatenation


```python
'1'+'2'
```




    '12'




```python
'Donkey'+'Bird'
```




    'DonkeyBird'




```python
'Donkey'+' '+'Bird'
```




    'Donkey Bird'



## Replication


```python
'12'*10
```




    '12121212121212121212'




```python
#This won't work
'Donkey'*'Bird'
#How can you multiply words? (you can but its just not automatic)
```


    ---------------------------------------------------------------------------

    TypeError                                 Traceback (most recent call last)

    <ipython-input-111-668b01e7b100> in <module>()
          1 #This won't work
    ----> 2 'Donkey'*'Bird'
          3 #How can you multiply words? (you can but its just not automatic)


    TypeError: can't multiply sequence by non-int of type 'str'


## Strip


```python
stuff='***BINGO***'
print('From ', stuff, 'to...', stuff.strip('*'))
```

    From  ***BINGO*** to... BINGO


You can also write the code like this so it is not confusing at first:


```python
stink='!!!YIKES!!!'
print('Before')
print(stink)
print('After')
stink.strip('!')
```

    Before
    !!!YIKES!!!
    After





    'YIKES'



## Split


```python
s="Let\'s split the words"
print(s)
```

    Let's split the words



```python
s.split(' ')

```




    ["Let's", 'split', 'the', 'words']



## Slicing


```python
word="hello"
word
```




    'hello'




```python
word[0:]
```




    'hello'




```python
#-1 is the last element of 'hello' so, -1 = 'o'
word[-1]
```




    'o'




```python
#here we have 0-1 where 1 is exclusive so it is not counted and only the first element is printed
word[0:1]
```




    'h'




```python
word[0:2]
```




    'he'




```python
#here we have 0:5 in incriments of :2
word[0:5:2]
```




    'hlo'




```python
#reverse uses extended slice syntax. 
#It works by doing [begin:end:step] 
#by leaving beging:end out and using -1 for step...
word[::-1]
```




    'olleh'



## Length or len


```python
print(len(word))
```

    5


## Count


```python
print(word.count("l"))
```

    2


## Starts and Ends with


```python
greeting = "Hello world!"
print(greeting.startswith("Hello"))
print(greeting.endswith("asdfasdfasdf"))
print(greeting.endswith("!"))
print(greeting.endswith("a bang"))
```

    True
    False
    True
    False


## Substring Testing


```python
word.find('el')
```




    1




```python
#finds the closest l between 8:11, return location 9
#.find(sub[, start[, end]])
greeting.find('l',8,11)
```




    9




```python
#finds the closest l between 8:11, return location 9
#.find(sub[, start[, end]]) returns -1 if sub is not found
#still fuzzy here TBH
greeting.find(s,8,11)
```




    -1



#### Be sure to check the documentation whenever you wanna manipulate strings in some particular fashion. There are many, many ways.

## Common List Functions
* Store data
* Iterate using loops
* Lists are mutable
* Use common list functions


```python
zlist = [11,22,33]

zlist
```




    [11, 22, 33]



### Append


```python
#let's append to the list and add 44
zlist.append(44)

zlist
```




    [11, 22, 33, 44]



### Pop


```python
#here (3) is the 4th element in the list
#it displays the and then pops it from the list 
zlist.pop(3)
```




    44



### Indexing


```python
zlist[0:3]
```




    [11, 22, 33]



### Remove


```python
print(zlist)

zlist.remove(33)

print(zlist)
```

    [11, 22, 33]
    [11, 22]


### Extend


```python
zlist1 = [11,22,33]
zlist2 = [44,55,66]

zlist1.extend(zlist2)

zlist1
```




    [11, 22, 33, 44, 55, 66]





<br><br>



# First lets understand zip

### Then: Zip it. Zip it good! 


```python
#This is a great example, easy to understand but not practical
first = ['Py','Joe','Flip']
last = ['Barrios','Blow','Phillips']

names = zip(first, last)

for a,b in names:
    print(a,b)
```

    Py Barrios
    Joe Blow
    Flip Phillips



```python
#Here we are using intergers instead of strings but again, not so practical
#notice the last 55 of x is not printed(self explanatory-ish)
x = [11,22,33,44,55]
y = [44,55,66,77]

newList = zip(x,y)

for a,b in newList:
    print(a,b)
```

    11 44
    22 55
    33 66
    44 77



```python
#Here we are compairing intergers instead of strings making it a little practical
x = [11,22,33,44,55]
y = [44,55,66,77]

newList = zip(x,y)

for a,b in newList:
    if a<b:
        print(b)
```

    44
    55
    66
    77


## Tuples
Unlike Lists, tuples are immutable. You can trust that tuples never change and they can take strings, intergers, floats and even lists.


```python
example_tuple = ("blouse", [8, 4, 6], (1, 2, 3))
print(example_tuple)

```

    ('blouse', [8, 4, 6], (1, 2, 3))



```python
#example_tuple[0]="blouse" example_tuple[1]=[8,4,6] and example_tuple[2]=(1, 2, 3)
#check it out

example_tuple[2]
```




    (1, 2, 3)




```python
#You can find out how many objects are inside of example_tuple like this:

count = 0
for i in example_tuple: #possible but remember that Tuples are immutable
        count+=1

print(count)
```

    3


## Dictionaries and Keys
Each key is separated from its value by a colon (:), the items are separated by commas, and the whole thing is enclosed in curly braces. An empty dictionary without any items is written with just two curly braces, like this: {}.

Keys are unique within a dictionary while values may not be. The values of a dictionary can be of any type, but the keys must be of an immutable data type such as strings, numbers, or tuples.


```python
dict = {'Name': 'Kiley', 'Age': 7, 'Class': 'First'}

print("dict['Name']: ", dict['Name'])
print("dict['Age']: ", dict['Age'])


    dict['Name']:  Kiley
    dict['Age']:  7
```
<br>

