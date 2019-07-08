<!---

<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/00-Table-of-Contents.md" rel="Return to TOC"> Return to TOC </a>

---
 
![](/01_pseudocode/assets/bookCover.png)

**Information used in this lesson topic and Figures shown are from the following source:** Farrell, Joyce, Programming Logic & Design (2017), comprehensive, 9th edition. Centage Learning, 20 Channel Center Street, Boston, MA 02210. USA
ISBN-10: 1-337-10207-5, ISBN-13: 978-1-337-10207-0

---

## Arrays

**Objective**

**In this section, you will learn about:**
* Arrays
* How an array can replace nested decisions
* Using constants with arrays
* Searching an array for an exact match
* Using parallel arrays
* Searching an array for a range match
* Remaining within array bounds
* Using a for loop to process arrays

## Arrays

**Array**
* A series or list of variables in computer memory
* All variables share the same name, and must be the same data type
* Each variable has a different subscript

## Computer Memory and Arrays

**Element: an item in the array**
**Array elements are contiguous in memory**
**Size of the array: the number of elements it will hold**
**Subscripts or indexes**
Position number of an item in an array starting from 0 to one less than the number of elements in array
Subscripts are always a sequence of integers
**Adding data values is called populating the array**

## Array Characteristics
**An array is a list of data items in contiguous memory locations**
**Each data item in an array is an element**
**Each array element is the same data type and the same size**
**Each element is differentiated from the others by a subscript, which is a whole number**
**Usable subscripts for an array range from 0 to one less than the number of elements in an array**
**Each array element can be used in the same way as a single item of the same data type**

## How an Array Can Replace Nested Decisions 

**The array reduces the number of statements needed**
**Six dependent count accumulators are redefined as a single array**
**Variable as a subscript to the array**
**Array subscript variable must be:**
Numeric with no decimal places
Initialized to 0
Incremented by 1 each time the logic passes through the loop

**The array reduces the number of statements needed**
**Six dependent count accumulators are redefined as a single array**
Figure 6-2
**Variable as a subscript to the array**
**Array subscript variable must be:**
Numeric with no decimal places
Initialized to 0
Incremented by 1 each time the logic passes through the loop

**Use constants in several ways:**
To hold the size of an array
As the array values
As subscripts

**Avoid “magic numbers” (unnamed constants)**
**Declare a named numeric constant to be used every time the array is accessed**
**Make sure any subscript remains less than the constant value**
**Constants are created automatically in many languages**

**Sometimes the values stored in arrays should be constants**
**Example**
```
	string MONTH[12] = "January", "February", "March", "April", "May", "June", "July", "August", "September", "October", "November", "December"
```

**vUse a numeric constant as a subscript to an array**
**Example**
Declare a named constant as: num INDIANA = 5
Display value with:
	output salesArray[INDIANA]

**Sometimes you must search through an entire array to find a value – called a linear search**
**Example: mail-order business**
Item numbers are three-digit, non-consecutive numbers
Customer orders an item; check if item number is valid
Create an array that holds valid item numbers
Search the array for an exact match

**Flag: a variable that indicates whether an event occurred**
**Technique for searching an array**
Set a subscript variable to 0 to start at the first element
Initialize a flag variable to false to indicate the desired value has not been found
Examine each element in the array
If the value matches, set the flag to True
If the value does not match, increment the subscript and examine the next array element

### Using Parallel Arrays
**Example: mail-order business**
Two arrays, each with six elements
Valid item numbers
Valid item prices
Each price in the valid item price array is in the same position as the corresponding item in the valid item number array
**Parallel arrays**
Each element in one array is associated with an element in the same relative position in the other array
**Look through the valid item array for the customer’s item
When a match is found, get the price from the item price array

![](/01_pseudocode/assets/parallelArrays.jpg)

### Parallel Arrays
Use parallel arrays when:
Two or more arrays contain related data
A subscript relates the arrays
Elements at the same position in each array are logically related
Indirect relationship
Relationship between an item’s number and its price
Parallel arrays are very useful

### Search Efficiency

The program should stop searching the array when a match is found 
Set a variable to a specific value instead of letting normal processing set it
Leaving a loop as soon as a match is found improves efficiency
The larger the array, the more beneficial it becomes to do an early exit

### Searching an Array for a Range Match
Programmers may want to work with ranges of values in arrays, 1 through 5 or 20 through 30
Example: mail-order business
Read the customer order data; determine the discount based on the quantity ordered
First approach
An array with as many elements as each possible order quantity
Store the appropriate discount for each possible order quantity
Drawbacks of previous approach
Requires a very large array; uses a lot of memory
Stores the same value repeatedly
How do you know when you have enough elements?
Customer can always order more
Better approach
Create two parallel arrays, each with four elements
One array has the four discount rates
One array has the low end of each quantity range
Use a loop to make comparisons

### Saying within Array Bounds
In bounds: using a subscript that is within the acceptable range for the array
Out of bounds: using a subscript that is not within the acceptable range for the array
An invalid array subscript is a logical error
When an invalid subscript is used:
Some languages stop execution and issue an error
Other languages access a memory location outside of the array
The program should prevent bounds errors
To improve a program, add a test to ensure the entered subscript is valid
If entered subscript is not valid:
Display an error message and end the program
Use a default value
Continuously prompt the user for a new value until it is valid
To improve a program, add a test to ensure the entered subscript is valid
If entered subscript is not valid:
Display an error message and end the program
Use a default value
Continuously reprompt the user for a new value until it is valid

### Using a *for* loop to Process an Array
for loop: a single statement
Initializes the loop control variable
Compares it to a limit
Alters it
The for loop is especially convenient when there is a need to process every element in the array
Must stay within array bounds
Highest usable subscript is one less than the array size

### Summary

Array: a named series or list of values in memory
Same data type
Different subscript
Use a variable as a subscript to the array to replace multiple nested decisions
Constants can be used to hold an array’s size
Searching through an array requires
Initializing a subscript
Using a loop to test each element
Setting a flag when a match is found
Parallel arrays: each element in one array is associated with the element in a second array
Elements in each array have the same relative position
For range comparisons, store either the low- or high-end value of each range
Access data in an array
Use a subscript containing a value that accesses memory within the array bounds
A subscript is out of bounds if it is not within the defined range of acceptable subscripts
The for loop is a convenient tool for working with arrays when processing each element of an array from beginning to end


















--->


