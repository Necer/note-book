数组列表

**

- Java only destroys unwanted objects when the last reference has been lost.
    
- Keeping references to unneeded objects is sometimes called loitering.
    
- Save memory. Don’t loiter.
    

**

loitering：
在栈的数组实现中有对象的引用，且该引用不再需要但仍被保留。
Java并不知道该引用不再需要，为了确保不被需要的引用被GC回收空间，需要置空(NULL)