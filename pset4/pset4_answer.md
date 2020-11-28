[Problem set 4 PDF](https://ocw.mit.edu/courses/electrical-engineering-and-computer-science/6-006-introduction-to-algorithms-fall-2011/assignments/MIT6_006F11_ps4.pdf)

# Problem 4.1

- [ ] (a) Hashing strings containing English phrases
  - [ ] What is the expected value shown in lecture of the algorithm performance?
- [ ] (b) True statements about 2 properties: correctness and performance  
  - False - Dynamic resizing alone will preserse both properties (because regardless of dynamic resizing, correntness can be violated if the load factor of the array is too high.)
  - False - Collision resolution alone will preserve performance, but not correctness (because collision resolution does not assure performance, for example, if the starting size of the dict is too small, we can have a lot of collisions and the later insertions take longer and longer time due to traversing time in case we simply use a linked-list of values for a key when collision happens.)
- [ ] (c) Best time complexity achieved by enlarging a table of size m into size m', table contains n elements.
  - [ ] Watch lecture on resizing.

# [x] Problem 4.2
(a) Membership testing use case can be described by "Many insertions right after creation, and then mostly lookups".

(b) For this use case alone, I would choose "A large minimum size, and a growth rate of 2" because there are many insertions   
- [x] What is minimum size? Starting size for any new dict.  
- [x] What is growth rate? The rate at which to grow the hash table when hitting max load. Max load can be 50-80% for example.  
- [Nice reference for python dict](https://stackoverflow.com/questions/56097997/how-does-python-implement-dictionaries)  

# Problem 4.3  

- [x] Implement `subsequenceHashes`.
- [x] Implement `Multidict` and verify with test cases
- [ ] Implement `getExactSubmatches` as generator, returns `(x,y)` indicating that k-length subsequences at position x in 1st input matches subsequences at position y in the 2nd input.
- [ ] Implement `intervalSubsequenceHashes`, which returns same thing as `subSequenceHashes` except that it hashes only 1 in m subsequences.
- [ ] Run comparisons between the two human samples (paternal and maternal) and between the paternal sample and each of the animal samples.