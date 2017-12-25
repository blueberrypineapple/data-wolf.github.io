# datawolf.us
Data Science Flashcards

## Quickstart

```python
def flashcard(my_num):
        import requests
        link = 'http://datawolf.us/card'+ str(my_num) +'.txt'
        f = requests.get(link)
        print(f.text)
```


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
