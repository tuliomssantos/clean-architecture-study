#   Dependency Inversion Principle

>   The Dependency Inversion Principle (DIP) tells us that the most flexible systems are those in which source code dependencies refer only to abstractions, not to concretions.

The implication, then, is that stable software architectures are those that avoid depending on volatile concretions, and that favor the use of stable abstract interfaces. This implication boils down to a set
of very specific coding practices: 

*   **Don’t refer to volatile concrete classes.** Refer to abstract interfaces instead.
*   **Don’t derive from volatile concrete classes**. This is a corollary to the previous rule, but it bears
special mention.
*   **Don’t override concrete functions**. Concrete functions often require source code dependencies.
*   **Never mention the name of anything concrete and volatile**. This is really just a restatement of
the principle itself.