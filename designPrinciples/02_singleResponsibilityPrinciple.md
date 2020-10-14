#   Single Responsibility Principle

***The SRP is the least well understood principle.***

A common mistake is to think that a module should do only one thing.

A function must do one thing. *"But it is not one of the SOLID principles—it is not the SRP".*

>   *A module should have one, and only one, reason to change*

We can think of it this way, a software module is made to satisfy a need of users or stakeholders. These users and stakeholders are the reason for changing the module.

>   *A module should be responsible to one, and only one, user or stakeholder.*

Unfortunately, users or stakeholders are not very suitable words as there may be more than one user or stakeholder who wants to be modified.

Therefore, we refer to a group. One or more people requiring change.

>  **A module should be responsible to one, and only one, actor.**

##  What is a module?
*Module is just a cohesive set of functions and data
structures.*

(An object ?)

So the SRP:
>  **A cohesive set of functions and data structures (like an object) should be responsible to one, and only one, actor**

---
##   Seeking to understand

Note that the explanation above relates the SRP directly to stakeholders.

> This means that we split code up based on the social structure of the users using it. 

References

*   [Is domain knowledge needed for the Single Responsibility Principle?](https://khalilstemmler.com/articles/solid-principles/single-responsibility/)

> **Understanding the domain is the entirely the point of Single Responsibility Principle.**

**It's necessary to know the domain to understand how to structure a module in different parts with a single responsibility.**