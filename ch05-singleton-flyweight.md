# Singleton Pattern

With the Singleton design pattern, you have only one object of a particular class throughout your code.

## REMEMBER

To make sure you only have one object, no matter how many times someone’s code tries to create more objects, use the Singleton design pattern.
Ensure a class only has one instance, and provide a global point of access to it.

You use the Singleton design pattern when you want to either restrict resource use.

## TIP

You can use the Singleton pattern when you want to restrict the number of objects created because you want to share the data in those object.

## TECHINICAL STUFF

Creating a single object can also be important when you’re multithreading and you don’t want conflicts in how the data behind that object is accessed.

## WARNING

Here’s something to be careful of — if you’re using multiple class loaders and singleton objects, you might end up with issues. Because each class loader uses its own namespace, you might in fact end up with multiple singleton objects. 

# FlyWeight Pattern

The Flyweight pattern is similar to the Singleton pattern. Here, however, the idea is that if your code uses many large objects — **using up system resources** — you can **fix things by using a smaller set of template objects** that can be configured on-the-fly to **look like those larger objects**. The **configurable objects — the flyweights** — are smaller and reusable (so there are fewer of them), but after being configured, they will appear to the rest of your code as though you still have many large objects.