# Difference between heap and stack memory.

Reference : http://javarevisited.blogspot.com/2013/01/difference-between-stack-and-heap-java.html <br>
Solution: <br>
1. Main difference between heap and stack is that stack memory is used to store local variables and function call, whereas heap memory is used to store objects in Java. 
No matter, where object is created in code e.g. as member variable, local variable or class variable,  they are always created inside heap space in Java.<br>
2. If you are using Recursion, on which method calls itself, You can quickly fill up stack memory. Another difference between stack and heap is that size of stack memory is lot lesser than size of  heap memory in Java. <br>
3. Variables stored in stacks are only visible to the owner Thread, while objects created in heap are visible to all thread. In other words stack memory is kind of private memory of Java Threads, while heap memory is shared among all threads.<br>
4. Different threads share the same heap (but different stacks).Each thread has its own stack. 
