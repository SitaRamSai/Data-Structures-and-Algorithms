## Types of Recursion

- Recursion is always in two phases, calling phase, returning phase. 

### Tail Recursion

When the recursion is not having anything do in the returning phase, then it is called as tail recursion. It basically is returning to its main origin without having to perform any operations. 

- Tail recursion can be easily converted to a loop.
- It is a best practice to convert to loop if we see any traces of tail recursion. 
- Recursion takes O(n) space complexity because it has to create n activation records, a loop will take only 1 activation record, it is not creating any -  - new activation records, 
  - Memory
  >> Recursion -> O(n)
  >> Loop -> O(1)

### Head Recursion

When the function call is the first call it is making without doing any operations, then it is a head recursion.


### Tree Recursion


