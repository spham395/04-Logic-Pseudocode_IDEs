Pseudocode PRACTICE
#1. Personal Info  
Declare name  
Declare address  
Declare telephoneNumber  
Declare collegeMajor  
  
Display Prompts  
Input data  
  
Display data  
  
#2. Sales Prediction  
Declare totalSales  
Declare profit  
  
Display "Enter projected amount of total sales"  
Input totalSales  
  
Set profit = totalSales * .23  
  
Display "$", profit, " profit from $", totalSales  
  
#3. Land Calculation  
start  
    Input totalSquareFeet  
    Set totalAcre = totalSquareFeet / 43560  
    Output totalAcre  
stop   
  
#4. Total Purchase   
start  
    Display "What is the price of each item?"  
    input item1  
    input item2  
    input item3  
    input item4  
    input item5  
    Set subTotal = item1 + item2 + item3 + item4 + item5  
    Set salesTax = subTotal * 0.06
    Set total = subTotal + salesTax  
    Output subTotal, salesTax, total  
stop
#5. Distance Traveled  
start  
    Set distanceFive = 5 * 60  
    Set distanceEight = 8 * 60  
    Set distanceTwelve = 12 * 60  
    Output "The distance the car will travel in 5 hours", distanceFive  
    Output "The distance the car will travel in 8 hours", distanceEight 
    Output "The distance the car will travel in 12 hours", distanceTwelve 
stop  

Stucture pseudocode 22 OCT 2019
lowerPen()
movePen()
rotate90()
raisePen()
movePen()
rotate90()
lowerPen()
movePen()
rotate90()
movePen()
rotate90()
raisePen()
movePen()
drawCircle()
rotate90()

# 24 OCT 2019
## Exercise Workbench Functions (DAY 4)

1. As shown in this chapter, write a pseudocode statement that generates a randomnumber in the range of 1 through 100 and assigns it to a variable named rand
```
Declare Integer rand = 0

Set rand = Random(1, 100)
```
2. The following pseudocode statement calls a function named half, which returns a value that is half that of the argument. (Assume both the result and number variables are Real.) Write pseudocode for the function. Set result = half(number)
```
Declare Real result = 0, number = ?

Set result = half(number)

Function Real half(Real argument)
    Return argument / 2
End Function
```
3. A pseudocode program contains the following function definition:
```
Function Integer cube(Integer num)   
    Return num * num * num
End Function
```
Write a statement that passes the value 4 to this function and assigns its return value to the variable result
```
Declare Integer result = 0

Set result = cube(4)
```
4. Design a pseudocode function named timesTen that accepts an Integer argument. When the function is called, it should return the value of its argument multiplied times 10.
```
Function Integer timesTen(Integer argument)
    return argument * 10
End Function
```
5. Design a pseudocode function named getFirstName that asks the user to enter his or her first name, and returns it.
```
Function String getFirstName()
    Declare String firstName
    Display "Enter your First Name"
    Input firstName
    Return firstName
End Function
```
6. Assume that a program has two String variables named str1 and str2. Write a pseudocode statement that assigns an all uppercase version of str1 to the str2 variable
```
Set str2 = ToUpper(str1)
```

### Debugging Exercises
1. Display random(7, 1) -> Display random(1, 7)
2. Return discount -> Return discountPrice
3. Call tenPercent(value) -> Assign