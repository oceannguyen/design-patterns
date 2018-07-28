# Template Method pattern

You use the Template Method design pattern when you’ve got an algorithm of
several steps and you want to allow customization by subclasses. It’s that
easy.

## TIP

You should use the Template Method pattern when you have an algorithm that is made of up multiple steps, 
and you want to be able to customize some of those steps

# Builder pattern

Use the Builder pattern when you want client code and have control over the construction process

## TIP

In the Template Method design pattern, the multi-step algorithm is king —
you set it up the way you want it, and all the subclasses have to follow your lead. 
But now the situation is different — the client wants to set the order and number of steps in the algorithm

## Remember

Use the Builder design pattern when you want client code to have control
over the construction process but want to be able to end up with different
kinds of objects (each of which is built by a different type of builder).
