# The big four OOP building blocks

There are four pillars of OOP — abstraction, encapsulation, polymorphism,
and inheritance.

## Abstraction is the good kind of breakdown

Abstraction isn’t a programming technique; in essence, it just means that you conceptualize
a problem before applying OOP techniques.

## Encapsulating all that junk

When you encapsulate functionality into an object, you decide what interface
that object exposes to the world.

## Mighty polymorphism rangers

The ability to write code that can work with different object types and decide 
on the actual object type at runtime.

## Inheritance without the pesky taxes

the process by which one class can inherit methods and properties from another

# Strategy Pattern

## Remember

Separate the parts of your code that will change the most from the rest of your application and
try to make them as freestanding as possible for easy maintenance. 
You should also always try to reuse those parts as much as possible.

On the other hand, you can extract the volatile parts of your code and
encapsulate them as objects, you can use those objects as you need them —
and the entire task is handled by the code in such an object, it’s not spread
out over generations of classes.

One object, one task often makes sense instead of writing multi-generation
code where one task is spread out over a dozen generations.

## Tip

When planning for change, consider “has-a” instead of “is-a” relationships,
and put volatile code in the objects your application contains, rather than
inheriting that code.

Consider using the Strategy design pattern if you have one of the following
situations:

- You have volatile code that you can separate out of your application 
for easy maintenance.
- You want to avoid muddling how you handle a task by having to split
implementation code over several inherited classes.
- You want to change the algorithm you use for a task at runtime.