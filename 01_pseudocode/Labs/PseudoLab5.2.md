# CHOOSE FOUR PROMPTS FROM THE LIST 

# Bug Collector

A bug collector collects bugs every day for seven days. Design a program that keeps a running total of the number of bugs collected during the seven days. The loop should ask for the number of bugs collected for each day, and when the loop is finished, the program should display the total number of bugs collected.

```
Declare Integer totalBugsOfDay, totalBugsOfWeek = 0
Constant Integer DAYS_IN_WEEK = 7

For day = 1 To DAYS_IN_WEEK
    Display "How many bugs did you catch today?\n"
    Input totalBugsOfDay
    Set totalBugsOfWeek += totalBugsOfDay
```

# Calories Burned

Running on a particular treadmill you burn 3.9 calories per minute. Design a program that uses a loop to display the number of calories burned after 10, 15, 20, 25, and 30 minutes.
```
Constant Real CPM_RATE = 3.9

For minutes = 10 To 30 Step 5
    Set caloriesBurned = minutes * CPM_RATE
    Display "At ", minutes, " minutes, you burned ", caloriesBurned, " calories."
```
# Budget Analysis

Design a program that asks the user to enter the amount that he or she has budgeted for a month. A loop should then prompt the user to enter each of his or her expenses for the month, and keep a running total. When the loop finishes, the program should display the amount that the user is over or under budget.
```
Declare Real Budget
Declare String anotherExpense = 'n'
Display "What is your budget for the month?"
Input Budget
Display "Enter expense(s)? (enter y)"
While anotherExpense == 'y'
    
```
# Sum of Numbers

Design a program with a loop that asks the user to enter a series of positive numbers. The user should enter a negative number to signal the end of the series. After all the positive numbers have been entered, the program should display their sum.

# Tuition Increase

At one college, the tuition for a full-time student is $6,000 per semester. It has been announced that the tuition will increase by 2 percent each year for the next five years. Design a program with a loop that displays the projected semester tuition amount for the next five years.

# Average Rainfall

Design a program that uses nested loops to collect data and calculate the average rainfall over a period of years. The program should first ask for the number of years. The outer loop will iterate once for each year. The inner loop will iterate twelve times, once for each month. Each iteration of the inner loop will ask the user for the inches of rainfall for that month. After alliterations, the program should display the number of months, the total inches of rainfall, and the average rainfall per month for the entire period.

# Celsius to Fahrenheit Table

Design a program that displays a table of the Celsius temperatures 0 through 20 and their Fahrenheit equivalents. The formula for converting a temperature from Celsius to Fahrenheit is

![image](https://user-images.githubusercontent.com/47218880/67429019-e7911f00-f5a4-11e9-849e-c07e34b8044c.png)

where F is the Fahrenheit temperature and C is the Celsius temperature. Your program must use a loop to display the table.

# Pennies for Pay

Design a program that calculates the amount of money a person would earn over a period of time if his or her salary is one penny the first day, two pennies the second day, and continues to double each day. The program should ask the user for the number of days. Display a table showing what the salary was for each day, and then show the total pay at the end of the period. The output should be displayed in a dollar amount, not the number of pennies.

# Largest and Smallest

Design a program with a loop that lets the user enter a series of numbers. The user should enter 
−
99
 to signal the end of the series. After all the numbers have been entered, the program should display the largest and smallest numbers entered.

# First and Last

Design a program that asks the user for a series of names (in no particular order). After the final person’s name has been entered, the program should display the name that is first alphabetically and the name that is last alphabetically. For example, if the user enters the names Kristin, Joel, Adam, Beth, Zeb, and Chris, the program would display Adam and Zeb.

# Calculating the Factorial of a Number

In mathematics, the notation n! represents the factorial of the nonnegative integer n. The factorial of n is the product of all the nonnegative integers from 1 up through n. For example:
![image](https://user-images.githubusercontent.com/47218880/67429154-2cb55100-f5a5-11e9-959b-79c4f1a34757.png)

and

![image](https://user-images.githubusercontent.com/47218880/67429177-3c349a00-f5a5-11e9-94c6-82826c1b03cf.png)

Design a program that asks the user to enter a nonnegative integer and then displays the factorial of that number.

# Multiplication Table

Design a program that uses nested loops to display a multiplication table for the numbers 1 through 12. The program’s output should look like this:
```
1 * 0 = 0

1 * 1 = 1

1 * 2 = 2

1 * 3 = 3
```
and so forth..
```
12 * 9 = 108

12 * 10 = 120

12 * 11 = 132

12 * 12 = 144
```
