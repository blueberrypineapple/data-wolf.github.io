---
layout: page
title: About Data Wolf
subtitle: A Data Science and Machine Learning virtual wolf
---
![IMG](https://github.com/data-wolf/data-wolf.github.io/blob/master/img/ava-icon.png?raw=true)
# Data Science Flashcards
Data Wolf presents [Data Science Flashcards!](https://datawolf.us/2017-10-10-data-science-flashcards/) I made these while taking UC San Diego's DSE200x course on edX and my favorite online bootcamp, DataCamp! For DataCamp I took Introduction to Python for Data Science and Intermediate Python for Data Science. The paper flashcards are made from MOO busniess cards and will be for sale soon while free version will be made available on Instagram. If you still want to learn using paper flashcards buy you don't have the budget for them, send me an email and I will send you a file so you can have them printed or you can print them on your home printer, school, local library or friends can also be a good resource. DIY option: Hand writing these flashcards onto 3X5 or 4X6 is highly reccomended, here is why:

1. I did it in Photoshop and I have become a better programer for it.
2. Once you really have them down, use it as a gift to get a friend or family member into Python.
3. After you given them away, you can quiz yourself on Instagram to make seure you still remember!

## Quickstart

Write this Python 3 function:
```python
def flashcard(my_num):
        import requests
        link = 'http://datawolf.us/card'+ str(my_num) +'.txt'
        f = requests.get(link)
        print(f.text)
```

To call this function type flashcard(1) as shown below. For single digit cards do not use 0. 

ie. 1 NOT 01 so flashcard(1)

```python
flashcard(1)
```

    >>> 35+16
    51
    >>> 25-16
    9
    >>> 3*5
    15
    >>> 10/2
    5.0
    >>> 2**7
    128
    >>> 18%7
    4



```python
flashcard(2)
```

    >>> movie = 10
    >>> popcorn = 25
    >>> movie + popcorn
    35
    



```python
flashcard(3)
```

    >>> a="This list"
    >>> b=" demonstrates concatenation."
    >>> my_list=a+b
    >>> print(my_list)
    This list demonstrates concatenation.
    

Etc...<br>

This project is still in progress, check back in 2018.
