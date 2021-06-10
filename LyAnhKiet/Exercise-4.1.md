Exercise 4.1

1. Chapter 3 contained the program Calc.java. It is available on the program listings page on the book website.
Calc currently implements one function: it adds two integers. Use test-driven design to add additional functionality to subtract two integers, multiply two integers, and divide two integers. First create a failing test for one of the new functionalities, modify the class until the test passes, then perform any refactoring needed. Repeat until all of the required functionality has been added to your new version of
Calc, an all tests pass.
Remember that in TDD, the tests determine the requirements. This means you must encode decisions such as whether the division method returns an integer or a floating point number in automated tests before modifying the software.Submit printouts of all tests, your final version of Calc, and a screenshot showing that all tests pass. Most importantly, include a narrative describing each TDD test created, the changes needed to make it pass, and any refactoring that was necessary.


Write the test first

```Java

import org.junit.*;
import static org.junit.Assert.*;

public class CalcTest
{
   @Test
   public void testAdd()
   {
      assertTrue ("Calc sum incorrect", 5 == Calc.add (2, 3));
   }
   
   @Test
   public void testSubtract()
   {
   	assertTrue ("Calc subtraction incorrect", 5 == Calc.subtract(7, 2));
   }
   
   @Test
   public void testMultiply()
   {
   	assertTrue("Calc multiplication incorrect", 6 == Calc.multiply(2, 3));
   }
   
   @Test
   public void testDivide()
   {
   	assertTrue("Calc division incorrect", 2 == Calc.divide(6,3));
   }
}
```

And then add new methods to the Calc class the satisfy the test

```Java

public class Calc
{
   static public int add (int a, int b)
   {
      return a + b;
   }
   
   static public int subtract (int a, int b)
   {
      return a - b;
   }
   
   static public int multiply (int a, int b)
   {
      return a * b;
   }
   
   static public double divide (int a, int b)
   {
      return a / b;
   }
}

```

