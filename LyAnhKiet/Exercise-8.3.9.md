Exercise 8.3.9

For the Quadratic program in Chapter 7, complete the test sets for the following coverage criteria by filling in the “don’t care” values. Make sure to ensure reachability. Then derive the expected output. Download the program, compile it, and run it with your resulting test cases to verify correct outputs.
(a) Predicate Coverage (PC)
(b) Clause Coverage (CC)
(c) Combinatorial Coverage (CoC)
(d) Correlated Active Clause Coverage (CACC)

### Predicate Coverage (PC)
There are 3 predicates:  
- p1: argv.length == 3  
- p2: ok == true  
- p3: D < 0.0  

Tests: Root (int A, int B, int C)
- t1: {3, 5, 3}
- t2: {1, 2, 1}
- t3: {1}  

*All the predicates only have one clause, so the test set satisfies all type of coverages*