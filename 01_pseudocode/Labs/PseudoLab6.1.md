## 1. What is an off-by-one error?
```
Constant Integer SIZE = 10
Declare Integer scores[SIZE]
For i = 1 To SIZE - 1
    ...
End For
```
## 2.  Look at the following pseudocode:
```
Constant Integer SIZE = 10
Declare Integer values[SIZE]
```
How many elements does the array have?  
10  
What is the subscript of the first element in the array?  
  0  
What is the subscript of the last element in the array?  
9  
## 3. Look at the following pseudocode:
```
Constant Integer SIZE = 3
Declare Integer numbers[SIZE] = 1, 2, 3
What value is stored in numbers[2]?
3
What value is stored in numbers[0]?
1
```

## 4. A program uses two parallel arrays named customerNumbers and balances. The customerNumbers array holds customer numbers and the balances array holds customer account balances. If a particular customer’s customer number is stored in customerNumbers[187], where would that customer’s account balance be stored?
187
## 5. Look at the following pseudocode array declaration:
```
Declare Real sales[8][10]
```
How many rows does the array have?  
8  
How many columns does the array have?  
10  
How many elements does the array have?  
80  
Write a pseudocode statement that stores a number in the last column of the last row in the array.
```
Declare Integer number

Set sales[7][9] = number
```
##  6. Write a pseudocode declaration for a String array initialized with the following strings: "Einstein", "Newton", "Copernicus", and "Kepler".
```
Declare String greatMinds[] = ["Einstein", "Newton", "Copernicus", and "Kepler"]
```
## 7. Assume names is an Integer array with 20 elements. Design a For loop that displays each element of the array.
```
Declare Integer names[20]

For each elem in names
    Display elem
End For
```
## 8. Assume the arrays numberArray1 and numberArray2 each have 100 elements. Design an algorithm that copies the values in numberArray1 to numberArray2.
```
For i = 0 To 99
    Set numberArray2[i] = numberArray1[i]
End For
```
## 9. Assume the following declarations appear in a pseudocode program:
```
Constant Integer SIZE = 100
Declare Integer firstArray[SIZE]
Declare Integer secondArray[SIZE]
```
Also, assume that values have been stored in each element of firstArray. Design an algorithm that copies the contents of firstArray to secondArray.
```
For i = 0 To SIZE - 1
    Set numberArray2[i] = numberArray1[i]
End For
```
## 10. Design an algorithm for a function that accepts an Integer array as an argument and returns the total of the values in the array.
```
Func Integer getTotal(Integer numbers[])
    Declare Integer total = 0
    For each num in numbers
        total += num
    End For
    return total
End Func
```
## 11. Write a pseudocode algorithm that uses the For Each loop to display all of the values in the following array:
```
Constant Integer SIZE = 10
Declare Integer values[SIZE] = 1, 2, 3, 4, 5, 6, 7, 8, 9, 10

For each num in values
    Display num
End For
```




