# datawolf.us
Data Science Flash Cards

## Quickstart
```
def flashcard(my_num):
  import requests
  link - 'https://datawolf.us/card'+ str(my_num) +'.txt'
  f = requests.get(link)
  print(f.text)
```

To get the answers directly from the command line, type:
```
flashcard(1)
```

This project is still in progress, check back in 2018.
