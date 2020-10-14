# Open-Closed Principle

> **A software artifact should be open for extension but closed for modification.**

> **In other words, the behavior of a software artifact ought to be extendible, without having to modify that artifact.**

##  Experimental Application

Develop an application that shows the results of a montly budget on a web page. 

Requirements:

*   The results should be viewed as the user scrolls down. 
*   Positive numbers must be in black and nagative numbers in red.

After that, suppose your boss brings a new requirement:

*   Budgets must be printed on a black and white printer.
*   10 budgets per page.
*   Negative numbers must be printed in parentheses.

> **Clearly, some new code must be written. But how much old code will have to change? A good software architecture would reduce the amount of changed code to the barest minimum. Ideally, zero.**