<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/00-Table-of-Contents.md" rel="Return to TOC"> Return to TOC </a>

---
 
![](/01_pseudocode/assets/bookCover.png)

**Information used in this lesson topic and Figures shown are from the following source:** Farrell, Joyce, Programming Logic & Design (2017), comprehensive, 9th edition. Centage Learning, 20 Channel Center Street, Boston, MA 02210. USA
ISBN-10: 1-337-10207-5, ISBN-13: 978-1-337-10207-0

---

## Making Decisions

**Objective**

**In this section, you will learn about:**

* Selection structure
* Relational comparison operators
* **AND** logic
* **OR** logic
* **NOT** logic
* Making selections within ranges
* Precedence when combining **AND** and **OR** operators
* case structure

---
## The Selection Structure

**Boolean expressions can be only true or false**

**Every computer decision yields a true-or-false, yes-or-no, 1-or-0 result**

**Used in every selection structure**

**Dual-alternative (or binary) selection structure**
* Provides an action for each of two possible outcomes

### The Dual-alternative Selection Structure

![](/01_pseudocode/assets/dualAlt1.jpg)

Programming Logic & Design (2017), 9th edition

**Single-alternative (or unary) selection structure**
  * Action is provided for only one outcome
  
### The Single-alternative Selection Structure

![](/01_pseudocode/assets/singleAlt2.jpg)

Programming Logic & Design (2017), 9th edition

**if-then-else decision**
* if-then clause
* Holds the action or actions that execute when the tested condition in the decision is true

**else clause**
* Executes only when the tested condition in the decision is false

---
## Using Relational Comparison Operators

**Relational comparison operators**
* Six types supported by all modern programming languages
* Two values compared can be either variables or constants but must be same data type

**Trivial expressions**
* Always evaluates to the same result

**Example:**
```
35 = 35?	TRUE
17 = 71?	FALSE
```
**Relational comparison operators**
* Equivalency operator: =
  * True when its operands are equal
* Greater-than operator: >
  * True when the left operand is greater than the right operand
* Less-than operator: <
  * True when the left operand is less than the right operand

**Relational comparison operators**
* Greater-than–or-equal-to operator: >=
  * True when the left operand is **greater** than or **equal** to the right operand
* Less-than–or-equal-to operator: <=
  * Evaluates as true when the left operand is less than or equal to the right operand
* Not-equal-to operator: <>
  * Evaluates as true when its operands are not equivalent 

---
## Understanding AND logic

**Compound condition**
* Asks multiple questions before an outcome is determined

**AND decision** 
* Requires that both of two tests evaluate to true
* Requires a nested decision (nested if) or a cascading if statement

---
## Nesting AND Decisions for Efficiency

**When nesting decisions**
* Either selection can come first

**Performance time can be improved by asking questions in the proper order**

**In an AND decision, first ask the question that is less likely to be true**
* Eliminates as many instances of the second decision as possible
* Speeds up processing time

---
## Avoiding Common Errors in an AND Selection

**Second decision must be made entirely within the first decision**

**In most programming languages, logical AND is a binary operator**
* Requires a complete Boolean expression on both sides

**Expressions should not be trivial**

---
## Understanding OR Logic

**OR decision**
* Take action when one or the other of two conditions is true

**Example:**
```
“Are you free for dinner Friday or Saturday?”
```

---
## Writing OR Selections for Efficiency

**May ask either question first**
* Both produce the same output but vary widely in number of questions asked

**If first question is true, no need to ask second**

**In an OR decision, first ask the question that is more likely to be true**
* Eliminate as many extra decisions as possible

---
## Using the OR Operator

**Conditional OR operator (simply an OR operator)**
* Ask two or more questions in a single comparison

**Only one Boolean expression in an OR selection must be true to produce a result of true**

**Question placed first will be asked first**
* Consider efficiency

**Computer can ask only one question at a time**

---
## Avoiding Common Errors in an OR Selection

**Second question must be a self-contained structure with one entry and exit point**

**Request for A and B in English logically means a request for A or B**

**Examples:**
```
“Add $20 to the bill of anyone who makes more than 100 calls and to anyone who has used more than 500 minutes”
“Add $20 to the bill of anyone who has made more than 100 calls or has used more than 500 minutes”
```

**Make sure Boolean expression are complete**

**Make sure that selections are structured**

**Make sure to use OR selections when they are required**

**Make sure that expression are not trivial**

---
## Understanding NOT Logic

**The NOT operator**
* Reverses the meaning of a Boolean expression
```
if NOT (age < 18) then
   output "Can register to vote"
Endif
```
* If NOT true, it is false
* If NOT false, it is true
* Is a unary operator
  * Takes only one operator

---
## Avoiding a Common Error in a NOT Expression

**Be careful not to create trivial expressions**

**Incorrect code:**
```
if NOT (employeeDept = 1) OR NOT (employeeDept = 2) then
    output "Employee is not in Department 1 or 2“
Endif
```

**Correct code:**
```
if NOT (employeeDept = 1 OR employeeDept = 2) then
   output "Employee is not in Department 1 or 2"
endif
```
---

## Avoiding Common Errors When Using Range Checks

**Avoid a dead or unreachable path**
* Don’t check for values that can never occur
* Requires some prior knowledge of the data

**Never ask a question if there is only one possible outcome**

**Avoid testing the same range limit multiple times**

---
## Understanding Precedence When Combining AND and OR Operators

**Combine multiple AND and OR operators in an expression**

**When multiple conditions must all be true, use multiple ANDs**

```
if score1 >= MIN_SCORE AND score2 >= MIN_SCORE AND score 3 >= MIN_SCORE then
		classGrade = "Pass"
	else 
		classGrade = "Fail"
	endif
```

**When only one of multiple conditions must be true, use multiple ORs**
```
if score1 >= MIN_SCORE OR score2 >= MIN_SCORE OR score3 >= MIN_SCORE then
		classGrade = "Pass"
	else
		classGrade = "Fail"
	endif
```

**When AND and OR operators are combined in the same statement, AND operators are evaluated first**
```
if age <= 16 OR age >= 61 AND 
 rating = "G"
```

**Use parentheses to correct logic and force evaluations to occur in the order desired**
```
if (age <= 16 OR age >= 61) 
AND rating = "G"
```
**Mixing AND and OR operators makes logic more complicated**

**Can avoid mixing AND and OR decisions by nesting if statements**

---
## Understanding the *case* Structure

**Case structure – specialized selection structure**

**Use when there are several distinct possible values for a single variable**

**And each value requires a different subsequent action**

**For a range check:**
* **Make comparisons with the highest or lowest values in each range**
* **Eliminate unnecessary or previously answered questions**
* **The AND operator takes precedence over the OR operator**
* **Case structure is a specialized selection structure that can be used when there are several distinct possible values for a single variable, and each value requires a different subsequent action**

---
## Summary

* **Decisions involve evaluating Boolean expressions**
* **Use relational operators to compare values**
* **An AND decision requires that both conditions be true to produce a true result**
* **In an AND decision, first ask the question that is less likely to be true**
* **An OR decision requires that either of the conditions be true to produce a true result**
* **In an OR decision, first ask the question that is more likely to be true**

---

<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/01_pseudocode/05_Looping.md" > Continue to Next Topic </a>
