# Decorator Pattern

The Strategy design pattern introduced in Chapter 2 is all about helping you
handle change by letting you select from a family of external algorithms
rather than having to rewrite your code. 

The Decorator pattern is similar, in that it allows you to write your code and
avoid modification, while still extending that code if needed. That’s one of the 
major design points that I want to emphasize.

The Decorator design pattern takes a different approach. Instead of using
external algorithms, this design pattern is all about using wrapper code to
extend your core code

**REMEMBER**

As much as possible, make your code closed for modification, but open for
extension. In other words, design your core code so that it doesn’t have to be
modified a lot, but may be extended as needed.

The formal definition of the Decorator pattern from the GoF book (Design
Patterns: Elements of Reusable Object-Oriented Software, 1995, Pearson
Education, Inc. Publishing as Pearson Addison Wesley) says you can,
“Attach additional responsibilities to an object dynamically. Decorators
provide a flexible alternative to subclassing for extending functionality.

**TECHNICAL STUFF**

When you use wrapper code to extend your core functionality and you don’t need to
modify that core functionality, you are essentially decorating the code.

# Factory Pattern

"The idea, they think, is simply that you have an object that creates other
objects"

TIP: You should derive all the objects your factory creates from the same base
class or interface so that code that uses the objects it creates doesn’t have to
be modified for each new object type.

## Factory Method Pattern

According to the GoF book, the Factory Method design pattern should “Define
an interface for creating an object, but **let subclasses decide** which class to
instantiate. Factory method lets a class defer instantiation to subclasses.

"having to rewrite FirstFactory every time you change it"

TIP: Consider the GoF Factory Method pattern when circumstances have gotten
decentralized enough so that many programmers who subclass your factory
class are overriding it so much that they’re changing it substantially

