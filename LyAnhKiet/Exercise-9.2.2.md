Exercise 9.2.2 

Answer questions (a) through (d) for the mutant on line 5 in the method findVal().
(a) If possible, find test inputs that do not reach the mutant.
(b) If possible, find test inputs that satisfy reachability but not infection for the mutant.
(c) If possible, find test inputs that satisfy infection, but not propagation for the mutant.
(d) If possible, find test inputs that strongly kill the mutants.

## Original

```Java
public static int findVal(int numbers[], int val)       
   {                                                       
      int findVal = -1;                                    

      for (int i=0; i<numbers.length; i++)                 
         if (numbers [i] == val)                         
            findVal = i;                                  
         return (findVal);                                    
   }
```

## Mutant

```Java
public static int findVal(int numbers[], int val)       
   {                                                       
      int findVal = -1;                                    

      for (int i=1; i<numbers.length; i++)                 
         if (numbers [i] == val)                         
            findVal = i;                                  
         return (findVal);                                    
   }
```

### a)

Impossible

### b)

Impossible

### c)

[-1, 1], 1

### d)

[1, 0], 1
