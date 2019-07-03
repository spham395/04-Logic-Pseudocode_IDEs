<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/00-Table-of-Contents.md" rel="Return to TOC"> Return to TOC </a>

---
 
![](/01_pseudocode/assets/bookCover.png)

**Information used in this lesson topic and Figures shown are from the following source:** Farrell, Joyce, Programming Logic & Design (2017), comprehensive, 9th edition. Centage Learning, 20 Channel Center Street, Boston, MA 02210. USA
ISBN-10: 1-337-10207-5, ISBN-13: 978-1-337-10207-0

## Understanding Structures

**Objective**

**In this section, you will learn about:**

* Unstructured spaghetti code disadvantages
* Three basic structures: sequence, selection, & loop
* Structuring a program using a priming input
* Why a structure
* Recognizing a structure
* Structuring and modularizing unstructured logic

---
## Unstructured Spaghetti Code Disadvantages

**Spaghetti code**
* Unstructured tangled web of program statements
* Often a complicated mess
* Programs often work but are difficult to read and maintain
* Confusing and prone to error (nearly impossible to debug)

**Unstructured programs**
* Do not follow the rules of structured logic

**Structured programs** 
* Follow the rules of structured logic

---
## Unstructured Spaghetti Code

### Spaghetti code logic for washing a dog
![](/01_pseudocode/assets/spaghetti1.jpg)

---
## Understanding the Three Basic Structures

**Structure**
* Basic unit of programming logic 
* Three types of structure include:
  * Sequence structure
  * Selection structure (decision structure)
  * Loop structure

**any program can be constructed using one or more of these three structures**

**Sequence structure**
* Perform actions or tasks in order
* No branching or skipping any task

**Selection structure (decision structure)**
* Ask a question, take one of two actions based on testing a condition. Known as evaluating a Boolean expression, a statement that is either true or false 
* Often called if-then-else
* Dual-alternative ifs or single-alternative ifs

**Loop structure**
* Repeat actions while a condition remains true

---
## The Selection Structure

**Dual-alternative ifs**
* Contains two alternatives
* The if-then-else structure
```
if someCondition is true then
	do oneProcess
else
	do theOtherProcess 
endif
```

**Single-alternative ifs**
```
if employee belongs to dentalPlan then
	deduct $40 from employeeGrossPay 
```
* An else clause is not required

**null case**
* Circumstance where nothing is done

---
## The Loop Structure

**Loop structure**
* Repeats a set of actions while a condition remains true
  * Loop body
* Also called repetition or iteration
* Condition is tested first in the most common form of loop
* The while…do or while loop

**Loop structure**
```
while testCondition continues to be true
	do someProcess 
endwhile
while you continue to be hungry
	take another bite of food
   	determine if you still feel hungry
endwhile
```

---
## Combining Structures

**Any individual task or step in a structure can be replaced by a structure**

**Nesting structures**
* Placing one structure within another
* Indent the nested structure’s statements

**Block**
* A group of statements that execute as a single unit

**Structured programs have the following characteristics:**
* Include only combinations of the three basic structures
* Each structure has a single entry point and a single exit point
* Structures can be stacked or connected to one another only at their entry or exit points
* Any structure can be nested within another structure

---
## Using a Priming Input to Structure a Program

**Priming input (or priming read)**
* Reads the first input data record
* Is outside the loop that reads the rest of the records
* Helps keep the program structured

**Analyze a flowchart for structure one step at a time**

**Watch for unstructured loops that do not follow this order**
* First ask a question
* Take action based on the answer
* Return to ask the question again

---
## Understading "Why" Structure

**Use structured programming for:**
* Clarity—unstructured programs are confusing
* Professionalism—other programmers expect it
* Efficiency—most languages support it
* Maintenance —other programmers find it easier to read
* Modularity —easily broken down into modules

**Structured programming is sometimes called goto-less programming**

---
## Summary

**Spaghetti code**
* Statements not following the rules of structured logic

**Three basic structures**
* Sequence, selection, and loop
* Combined by stacking and nesting

**Priming input**
* Statement that reads the first input value prior to starting a structured loop

**Structured techniques promote:** 
* Clarity
* Professionalism
* Efficiency
* Modularity

**Flowcharts can be made structured by untangling logic**

**Logical steps can be rewritten to conform to the three structures: sequence, selection, and loop**

<a href="https://github.com/CyberTrainingUSAF/04-IDE-s-and-Algorithms-Pt.-1/blob/master/01_pseudocode/04_Decisions.md" > Continue to Next Topic </a>
