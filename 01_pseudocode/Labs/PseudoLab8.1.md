# Choose Two additional Programming Projects along with the (Mandatory) one. (Three Total) 

##  Payroll Program with Input Validation


Design a payroll program that prompts the user to enter an employee’s hourly pay rate and the number of hours worked. Validate the user’s input so that only pay rates in the range of $7.50 through $18.25 and hours in the range of 0 through 40 are accepted. The program should display the employee’s gross pay.
```
Start
	Display "$" + grossPay()
Stop

Func Real getHourlyPay()
	do
		Display "Enter a valid hourly pay rate"
		Input hourlyPay
	while(hourlyPay < 7.50 OR hourlyPay > 18.25)
	return hourlyPay
End Func

Func Integer getHoursWorked
	do
		Display "Enter a valid number of hours worked"
		Input hoursWorked
	while(hoursWorked < 0 OR hoursWorked > 40)
	return hoursWorked
End Func

Func Real grossPay()
	return getHourlyPay() * getHoursWorked()
End Func
```
## Theater Seating Revenue with Input Validation

A dramatic theater has three seating sections, and it charges the following prices for tickets in each section: section A seats cost $20 each, section B seats cost $15 each, and section C seats cost $10 each. The theater has 300 seats in section A, 500 seats in section B, and 200 seats in section C. Design a program that asks for the number of tickets sold in each section and then displays the amount of income generated from ticket sales. The program should validate the numbers that are entered for each section.
```
Constant Integer SEATS_SECTION_A = 300, SEATS_SECTION_B = 500, SEATS_SECTION_C = 200
Declare Integer total

total = calcSectionCost("A") + calcSectionCost("B") + calcSectionCost("C")

Display "Total sale of tickets is " total

Func Integer calcSectionCost(String section)
	if section == "A" then
		do
			Display "Enter amount of tickets sold in Section " + section
			Input seatsSold
		while seatsSold < SEATS_SECTION_A
		return SEATS_SECTION_A * seats
	else if section == "B" then
		do
			Display "Enter amount of tickets sold in Section " + section
			Input seatsSold
		while seatsSold < SEATS_SECTION_B
		return SEATS_SECTION_B * seats
	else if section == "C" then
		do
			Display "Enter amount of tickets sold in Section " + section
			Input seatsSold
		while seatsSold < SEATS_SECTION_C
		return SEATS_SECTION_C * seats
	return 0
End Func
Func validateSeats()
	do
		Display "Enter amount of tickets sold in Section " + section
		Input seatsSold
	while seatsSold < SEATS_SECTION_A
End Func
```
## Fat Gram Calculator

Design a program that asks for the number of fat grams and calories in a food item. Validate the input as follows:

Make sure the number of fat grams and calories is not less than 0.

According to nutritional formulas, the number of calories cannot exceed "fat grams X 9 "

Make sure that the number of calories entered is not greater than "fat grams X 9"

Once correct data has been entered, the program should calculate and display the percentage of calories that come from fat. Use the following formula:

![image](https://user-images.githubusercontent.com/47218880/67504468-0ba93a80-f64f-11e9-85d0-f080ac66a64a.png)

Some nutritionists classify a food as “low fat” if less than 30 percent of its calories come from fat. If the results of this formula are less than 0.3, the program should display a message indicating the food is low in fat.

## Speeding Violation Calculator

Design a program that calculates and displays the number of miles per hour over the speed limit that a speeding driver was doing. The program should ask for the speed limit and the driver’s speed. Validate the input as follows:

The speed limit should be at least 20, but not greater than 70.

The driver’s speed should be at least the value entered for the speed limit ­(otherwise the driver was not speeding).
Once correct data has been entered, the program should calculate and display the number of miles per hour over the speed limit that the driver was doing.
```
Start
	Display f"You were doing {0} mph over the speed limit",  calcSpeedLimitViolation()
Stop

Func Integer getSpeedLimit()
	Declare speedLimit
	do
		Display "Enter a valid speed limit"
		Input speedLimit
	while (speedLimit < 20 OR speedLimit > 70)
	return speedLimit
End Func

Func Integer getDriverSpeed(Integer speedLimit)
	Declare driverSpeed
	do
		Display "Enter a valid driver's speed"
		Input driverSpeed
	while (driverSpeed <= speedLimit)
	return driverSpeed
End Func

Func Integer calcSpeedLimitViolation()
	Declare Integer speedLimit, driverSpeed, amountViolated
	speedLimit = getSpeedLimit()
	driverSpeed = getDriverSpeed(speedLimit)
	amountViolated = driverSpeed - speedLimit
	return amountViolated
End Func
```
# Rock, Paper, Scissors Modification (MANDATORY)

In a previous Programming Exercise option you were asked to design a program that plays the Rock, Paper, Scissors game. In the program, the user enters one of the three strings—"rock", "paper", or "scissors"—at the keyboard. Add input validation (with a case-insensitive comparison) to make sure the user enters one of those strings only.
(If you didnt design one, here is a version of that game program to work with) 

### Program "Rock,Paper,Scissors"

```
// main module
Module main()
// Local variables
Declare Integer computer
Declare String player

// Get computer number
Set computer = Rand(1, 3)

// Get player number
Call getNumber(player)

// Show winner
Call showWinner(computer, player)

End Module

// The getNumber module gets an integer
Module getNumber(String Ref inputAnswer)
	//changes
	do
		Display “Enter rock, paper, or scissors:  “
		Input inputAnswer
	until (ToLower(inputAnswer) == "rock" OR ToLower(inputAnswer) == "[paper]" OR ToLower(inputAnswer) == "scissors" )
End Module

// The showWinner module shows if number is a prime
Module showWinner(Integer computer, String player)
	Declare Integer which
	Declare String computerString

	Set computerString = whichChoice(computer)
	Display “Computer chose “, computerString
	Set which = whoWon(computerString, player)
	If which == 1 Then
		Display “Computer wins.”
	Else If which == 2 Then
		Display “Player wins.”
	Else
		Display “No winner.”
	End If

End Module

// The whichChoice function displays choice 
Function String whichChoice (Integer number)

If number == 1 Then
	Return “rock”
Else If number == 2 Then
	Return “paper”
Else
	Return “scissors
End If

End Function

// The whoWon function selects winner 
Function Integer whoWon(String computerString, String player)
// 1 = rock, 2 = paper, 3 = scissors
// rock smashes scissors
// scissors cuts paper
// paper wraps rock

	// both choose same no winner
	If computer == player then
		Return 0
	End If

		// test computer chose rock
	If computer == "rock" then
		If player == "paper" then
			Return 2  // paper wraps rock
		Else If player == "scissors" then
			Return 1  // rock smashes scissors
		End If
		// test computer chose paper
	Else If computer == "paper" then
		If player == "rock" then
			Return 1  // paper wraps rock
		Else If player == "scissors" then
			Return 2  // scissors cuts paper
		End If
		// test computer chose scissors
	Else If computer == "scissors" then
		If player == "rock" then
			Return 2  // rock smashes scissors 
		Else If player == "paper" then
			Return 1  // scissors cuts paper
		End If
	End If

	Return 0

End Function
```
