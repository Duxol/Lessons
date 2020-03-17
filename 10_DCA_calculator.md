# Lessons from making "DCA calculator":  
## list(dictionary.keys()).index()
The following line finds the index of our desired dictionary item in our dictionary: 

`index_start = list(dictionary.keys()).index(start_item)`  
`index_end = list(dictionary.keys()).index(end_item)`  

For example I want to find the index of "2018-02-12"


## Importing a dictionary froma a txt file (ast module)

The 'ast' module allows to import a dictionary from a *.txt file

This method is prefered to regular eval() because it's safer --> google it

```
with open("output.txt") as file:  
    f = file.read()  
    dictionary = ast.literal_eval(f)
```

## Slicing a dictionary

To slice a dictionary use `itertools.islice()`  

This code creates a new dictionary by slicing an existing one to contain values from a starting point (index_start) to the stop point (index_stop)  

`sliced = dict(itertools.islice(dictionary.items(), index_stop, index_start))`


## Tracking the index in a for loop  
```
for idx, item in enumarate(list):
    print(idx)
    print(item)
```
