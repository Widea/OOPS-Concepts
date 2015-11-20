# What is type erasure?
=> Reference:<br>

Generics were introduced to the Java language to provide tighter type checks at compile time and to support generic programming. To implement generics, the Java compiler applies type erasure to:<br>

=> Replace all type parameters in generic types with their bounds or Object if the type parameters are unbounded. The produced bytecode, therefore, contains only ordinary classes, interfaces, and methods.<br>
=> Insert type casts if necessary to preserve type safety.<br>
=> Generate bridge methods to preserve polymorphism in extended generic types.<br>
Type erasure ensures that no new classes are created for parameterized types; consequently, generics incur no runtime overhead.



