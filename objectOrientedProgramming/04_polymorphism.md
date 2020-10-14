#   Polimorphism

What’s so great about polymorphism? To better appreciate its charms, let’s reconsider the example
copy program. What happens to that program if a new IO device is created? Suppose we want to use
the copy program to copy data from a handwriting recognition device to a speech synthesizer device:
How do we need to change the copy program to get it to work with those new devices?

We don’t need any changes at all! Indeed, we don’t even need to recompile the copy program. Why?
Because the source code of the copy program does not depend on the source code of the IO drivers.
As long as those IO drivers implement the five standard functions defined by FILE, the copy program
will be happy to use them.

##  Dependency Inversion

![figure8](/images/figure8.png)

When polymorphism is brought into play, however, something very different can happen

![figure9](/images/figure9.png)

In Figure, module HL1 calls the F() function in module ML1. The fact that it calls this function
through an interface is a source code contrivance. At runtime, the interface doesn’t exist. HL1 simply
calls F() within ML1.

Note, however, that the source code dependency (the inheritance relationship) between ML1 and the
interface I points in the opposite direction compared to the flow of control. This is called
dependency inversion, and its implications for the software architect are profound.

**The fact that OO languages provide safe and convenient polymorphism means that any source code
dependency, no matter where it is, can be inverted.**

With this approach, software architects working in systems written in OO languages have absolute
control over the direction of all source code dependencies in the system. They are not constrained to
align those dependencies with the flow of control. No matter which module does the calling and
which module is called, the software architect can point the source code dependency in either
direction.

**That is power!**