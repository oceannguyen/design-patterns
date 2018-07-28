# Adapter Pattern

Adapter lets classes work together that couldn’t otherwise because of incompatible interfaces.

## Remember
Convert the interface of a class into another interface the client expects. Adapter lets classes work together that couldn’t otherwise because of incompatible interfaces.

This design pattern is particularly good when you’re working with legacy code that can’t be changed, while the software that interacts with that code does change.

An adapter uses composition to store the object it’s supposed to adapt, and when the adapter’s methods are called, it translates those calls into something the adapted object can understand and passes the calls on to the adapted object.

There is another kind of adapter that is class adapter. "So object adapters rely on object composition, while class adapters rely on inheritance". Object adapters can be more flexible because they can work with not just the objects they’ve been designed to adapt but also subclassed objects of the adapted objects

# Facade Pattern

Facade defines a higher-level interface that makes the subsystem easier to use.

The Facade pattern gives you a wrapper that makes the original code easier to deal with.

If an object or class interface is too hard to work with, the Facade pattern gives you a front end to that interface to make it easier.

## Remember
Facade defines a higher-level interface that makes the subsystem easier to use.
Although using a Facade can fix the problem, it adds another layer, and if the underlying code changes, you’re going to have to change your Facade pattern as well.

## Tip

If one object needs to know too much about another to make their coupling loose, a Facade pattern can help.
Always go for the loosest coupling you can.