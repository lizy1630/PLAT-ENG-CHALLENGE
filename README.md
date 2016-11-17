# PLAT-ENG-CHALLENGE
1. Coding task:

To implement this, I used two immutable stacks to perform the immutable queue functions (in and out). 
So when out stack is used up, then reverse in stack as out stack, and clear in stack.
I also investigate how scala does it on its own. Interestingly, scala has built-in immutable list which can better perform the job of the stacks I used here. Core idea is the same, using two immutable lists as in and out stream, when out steam drains, replaces it with in.reverse and empty the in stream. 
Further study is I tried to find similar solution in java, but there is no built-in immutable collectionsin java, ```Collections.unmodifiableList(java.util.List<? extends T>) ```  is not immutable actually. However, guava has immutable list, so it may implement the queue in the same way scala does.

> https://google.github.io/guava/releases/snapshot/api/docs/com/google/common/collect/ImmutableList.html




2. Design Question: Design A Google Analytic like Backend System.

See the image file.

   
