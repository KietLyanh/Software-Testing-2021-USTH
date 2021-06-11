Exercise 7.2.2.7

**Answer questions a–d for the graph defined by the following sets:** <br>
**N = {1, 2, 3}** <br>
**N0 = {1}** <br>
**Nf = {3}** <br>
**E = {(1, 2), (1, 3), (2, 1), (2, 3), (3, 1)}** <br>
**Also consider the following (candidate) paths:** <br>
**p1 = [1, 2, 3, 1]** <br>
**p2 = [1, 3, 1, 2, 3]** <br>
**p3 = [1, 2, 3, 1, 2, 1, 3]** <br>
**p4 = [2, 3, 1, 3]** <br>
**p5 = [1, 2, 3, 2, 3]** <br>

**(a) Which of the listed paths are test paths? For any path that is not a test path, explain why not.** <br>

**(b) List the eight test requirements for Edge-Pair Coverage (only the length two subpaths).** <br>

**(c) Does the set of test paths from part (a) above satisfy Edge-Pair Coverage? If not, state what is missing.** <br>

**(d) Consider the prime path [3, 1, 3] and path p2. Does p2 tour the prime path directly? With a sidetrip?** <br>


### a)

p5 is not a test path because there is no way to reach 2 from 3 directly

### b)

|Test Paths|	Test Requirements that are toured by test paths directly|
|---|---|
|[1,3,1,2,3]|	[1,3,1], [1,2,3], [3,1,2]|
|[1,2,1,2,3]|	[1,2,3], [1,2,1], [2,1,2]|
|[1,2,3,1,2,3]|	[1,2,3], [2,3,1], [3,1,2]|
|[1,2,1,3]|	[1,2,1], [2,1,3]|
|[1,2,3,1,3]|	[1,2,3], [2,3,1], [3,1,3]|

### c)

From b), p1, p4 don't satisfy

### d)

No

With a sidetrip: [3, 1, 2, 1, 3]
