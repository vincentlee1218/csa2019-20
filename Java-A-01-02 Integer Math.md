# AP Computer Science A

## 1.2 Integer Math

# Integer Math

The following operations are support in Java Integers
1. Addition : +
2. Multiplication: *
3. Subtraction: -
4. Division: /
5. Remainder: % (use to find divisibility)
6. THERE IS NO EXPONENTIATION.  More on that.

# Math Operations

* Adding  (or subtracting or multiplying or dividing ) two  integers  does nothing.
* `2+3` does nothing.  You need to “store” the results.
```
int  result;
result=2+3;
```
Now `result` contains the value 5.

# Modifying a variable

* If you want to change the value of a variable by a quantity, you must modify the variable then assign the result back to the variable.
```
int result=5;
result = result+7;
```
# Short Cuts: Unary Operators

```
X+=5   short cut for x=x+5
X-=5   short cut for x=x-5
x/=5   short cut for x=x/5
x*=5   short cut for x=x*5
x++ short cut for x=x+1
X–- short cut for x=x-1
++x and --x also exist but are beyond the scope of this course.
```

# Craziness

* Integer operations always result in an integer.  This is okay for most cases but it cause problems for division
```
int X=12;
x/=5;
```
X is 2 not 2.4

Results are truncated (not rounded)

# Java Exercises

1. Write a Java program to print 'Hello' on scren and then print your name on a separate line.
2. Write a Java program to print the sum of 62 and 122 and -13.
3. Write a Java program to do the following
   1. -5 + 8 * 6
   2. (55 + 0) % 9
   3. 20 + -3 * 5 / 8
   4. 5 + 15 / 3 * 2 - 8 % 3
4. Write a Java program that takes two numbers as input and type its average

# More exercises

1. Write a java program to print the sum (addition), multiply, subract, divide and remainder of 125 and 25
2. Write a Java program that takes a number as iput and prints its multiplication table up to 10.
3. Write a Java program to take a number x as input and compute -2x^2 + 5x - 3
