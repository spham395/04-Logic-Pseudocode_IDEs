# Exercise Workbench
* Design a While loop that lets the user enter a number. The number should be multiplied by 10, and the result stored in a variable named product. The loop should iterate as long as product contains a value less than 100.
```
Declare Integer product = 0
While product < 100
   Display "Enter a number: "
   Input number
   Set product = number * 10
```
* Design a Do-While loop that asks the user to enter two numbers. The numbers should be added and the sum displayed. The loop should ask the user whether he or she wishes to perform the operation again. If so, the loop should repeat; otherwise it should terminate.
```
String again
Do
   Display "Enter two numbers: "
   Input number1, number2
   Set sum = number1 + number2
   Display "Go again? (enter y)"
   Input again
While again == 'y'
```
* Design a For loop that displays the following set of numbers:

0, 10, 20, 30, 40, 50, . . . , 1000
```
For number = 0 To 1001 Step 10
   Display number, "\n"
```
* Design a loop that asks the user to enter a number. The loop should iterate 10 times and keep a running total of the numbers entered.
```
Declare Integer total = 0
For count = 0 To 10
   Display "Enter a number: "
   Input number
   Set total += number
```
* Design a For loop that calculates the total of the following series of numbers:
![image](https://user-images.githubusercontent.com/47218880/67423054-31740800-f599-11e9-9565-031c1f729e1c.png)
```
Declare Integer bottom = 30
Declare Real total = 0
For top = 1 To 30
   Set total += top/bottom
   bottom -= 1
```
* Design a nested loop that displays 10 rows of # characters. There should be 15 # characters in each row.
```
For row = 0 To 10
   For col = 0 To 15
      Display "#"
```
* Convert the While loop in the following code to a Do-While loop:
```
Declare Integer x = 1
While x > 0
   Display "Enter a number."
   Input x
End While
```
```
Declare Integer x = 1
do
   Display "Enter a number."
   Input x
While x > 0
End While
```
* Convert the Do-While loop in the following code to a While loop:
```
Declare String sure
Do
  Display "Are you sure you want to quit?"
  Input sure
While sure != "Y" AND sure != "y"
```
```
Declare String sure
While sure != "Y" AND sure != "y"
  Display "Are you sure you want to quit?"
  Input sure
End While
```
* Convert the following While loop to a For loop:
```
Declare Integer count = 0
While count < 50
   Display "The count is ", count
   Set count = count + 1
End While
```
```
For count = 0 To 50
   Display "The count is ", count
End For
```
* Convert the following For loop to a While loop:
```
Declare Integer count
For count = 1 To 50
   Display count
End For
```
```
Declare Integer count = 1
While count < 50
   Display Count
   Set count += 1
End While
```
