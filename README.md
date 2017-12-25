# Data Science Flashcards
Data Wolf Flashcards are made from MOO sized business cards and will be for sale soon. Free versions are available on [Data Wolf Instagram](https://www.instagram.com/datawolf.us/). If you would like to learn with paper but money is an obstacle, send me an email and I will send you a zip file which you can print yourself or get printed at school, local library or with the help of a friends or family member. The DIY route: Writting each Data Science flashcard by hand on 3X5 or 4X6 cards will not only give you the best bang for your buck but you will be a better Data Scientist for it! I made these in Photoshop and it helped me a great deal.

## Getting Started:
1. Get paper flashcards!
2. Go green with [Data Wolf Instagram](https://www.instagram.com/datawolf.us/).
3. Follow Quickstart instructions below.

## Quickstart

1. Write this Python 3 function as printed below:

```python
def flashcard(my_num):
        import requests
        link = 'http://datawolf.us/card'+ str(my_num) +'.txt'
        f = requests.get(link)
        print(f.text)
```

2. Call this function with your card number. For single digits don't use 0, just 1-9.

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
    

3. Scan the QR on the card.
![IMG](https://github.com/data-wolf/data-wolf.github.io/blob/master/img/Screen%20Shot.png?raw=true)

Thank you for learning Data Science with Data Wolf!
This project is still in progress, so please check back in 2018.
