## Iterator Pattern

### Situation: These days, you have all kinds of collections to work with - trees, binary trees, arrays, ring buffers, hashes, hash maps, array lists, and many more. The ways these collections store their data internally vary a great deal, and if you want to access that data in the same way as these collections do internally you have to learn a different teachnique for every collection type.
*That’s where the Iterator comes in*

Iterators are designed to let you handle many different kinds of collections by accessing their members in a standard, accepted way, withou having to know the iternal details of those collections

**Tip**: The Iterator design pattern is especially important when the collection you're creating is made up internally of subcollections, as when you've mixed hashes with array lists, for example.

**TECHINIAL STUFF**:
- Why aren't iterators built into the collections they work with? They could be, but the design insight here is one of what's called single responsibility - a class should have only one thing to to.

## Composite Pattern

### Situation: The Composite design pattern is also about collections. With the Composite pattern, the idea is that you can create tree-like structures where each item in the tree - a single leaf with no children, or an entire branch with many children can be handled in the same way.

Composite pattern is designed to let you handle different types of objects in the same collection in the same way, and iterators fit in naturally here - to handle the elements of a tree branch, for example, you can iterate over them.

**Remember**: Compose objects into tree structures to represent part-whole hierarchies. Composite lets clients treat individual objects and compositions of objects uniformly.

The insight behind the Composite pattern is really about treating the leaves and branches in a tree-like structure the same way, not about tree structures. That makes it a heck of a lot easier to work with complex structures like trees beacause you don't have to use a different set of methods with a part of the structure compared to the whole.

*TIP*: To implement the Composite pattern, the GoF suggests that you use an abstract class as the basis for both the leaves and branches in the tree. Doing so gaives the leaves and branches a common set of methods, which is what the Composite patter is all about.