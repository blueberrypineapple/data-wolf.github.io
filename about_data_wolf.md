---
layout: page
title: About Data Wolf
subtitle: A Data Science and Machine Learning virtual wolf
---

# Data Science Flashcards

## Instructions
Data Wolf presents [Data Science Flashcards!](https://datawolf.us/2017-10-10-data-science-flashcards/) I made these while taking [UC San Diego's DSE200x](https://www.edx.org/micromasters/data-science) course on edX and working with my favorite online bootcamp, DataCamp! For DataCamp I took [Intro to Python for Data Science](https://www.datacamp.com/courses/intro-to-python-for-data-science) and [Intermediate Python for Data Science](https://www.datacamp.com/courses/intermediate-python-for-data-science). The paper flashcards are made from MOO busniess cards and will be for sale soon while the free version will be made available on Instagram. If you still want to learn using paper flashcards and money is an obstacle, send me an email and I will send you a file so you can have them printed or you can print them at home, school, local library or with the help of a friend. The Hardcore DIY option: Hand writting these flashcards onto 3X5 or 4X6 is highly reccomended, here is why:

1. I made these in Photoshop and while it took a while, I have become a  much better programmer for it.
2. Once you really have these down, use them as a gift to get a friend or family member into Python.
3. After you given them away, you can still quiz yourself on Instagram to make sure you still remember!

## Getting Answers: 

1. Write this Python 3 function:
```python
def flashcard(my_num):
        import requests
        link = 'http://datawolf.us/card'+ str(my_num) +'.txt'
        f = requests.get(link)
        print(f.text)
```

2. Call this function by typing flashcard(1) in the shell as shown below. For single digit cards do not use 0. 

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
