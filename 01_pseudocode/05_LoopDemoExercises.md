
# Program 5-1
```
 1  // Variable declarations
 2  Declare Real sales, commission
 3  Declare String keepGoing = "y"
 4
 5  // Constant for the commission rate
 6  Constant Real COMMISSION_RATE = 0.10
 7
 8  While keepGoing == "y"
 9      // Get the amount of sales.
10      Display "Enter the amount of sales."
11      Input sales
12
13      // Calculate the commission.
14      Set commission = sales * COMMISSION_RATE
15
16      // Display the commission
17      Display "The commission is $", commission
18
19      Display "Do you want to calculate another"
20      Display "commission? (Enter y for yes.)"
21      Input keepGoing
22  End While
```
```
Program Output (with Input Shown in Bold)
Enter the amount of sales.
10000.00 [Enter] 
The commission is $1000
Do you want to calculate another
commission? (Enter y for yes.)
y [Enter] 
Enter the amount of sales.
5000.00 [Enter] 
The commission is $500
Do you want to calculate another
commission? (Enter y for yes.)
y [Enter] 
Enter the amount of sales.
12000.00  [Enter] 
The commission is $1200
Do you want to calculate another
commission? (Enter y for yes.)
n [Enter]
```
