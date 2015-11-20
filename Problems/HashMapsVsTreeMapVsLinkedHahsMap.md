# Difference between Hashmap, TreeMap and Linked HashMap?
=> Reference: https://stackoverflow.com/questions/2889777/difference-between-hashmap-linkedhashmap-and-treemap<br>

All three classes implement the Map interface and offer mostly the same functionality. The most important difference is the order in which iteration through the entries will happen:<br>
=> HashMap makes absolutely no guarantees about the iteration order. It can (and will) even change completely when new elements are added.<br>
=>TreeMap will iterate according to the "natural ordering" of the keys according to their compareTo() method (or an externally supplied Comparator). Additionally, it implements the SortedMap interface, which contains methods that depend on this sort order.<br>
=>LinkedHashMap will iterate in the order in which the entries were put into the map<br>

"Hashtable" is the generic name for hash-based maps. In the context of the Java API, Hashtable is an obsolete class from the days of Java 1.1 before the collections framework existed. It should not be used anymore, because its API is cluttered with obsolete methods that duplicate functionality, and its methods are synchronized (which can decrease performance and is generally useless). Use ConcurrrentHashMap instead of Hashtable.

