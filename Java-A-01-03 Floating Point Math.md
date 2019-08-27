# AP Computer Science A

## 1.3 Floating Point Math

# Floating Point Math

Java has many ways of representing floating points (real numbers).  They are `float, double, Math.Float, Math.Double`.

Today we are only going to focus on the primitive type `double`.  We will study `Math.Double` next semester.  

These two are in the AP test and you will be held accountable for them on the test.

The following basic operations are supported in Java floating points:
1. Addition : +
2. Multiplication: *
3. Subtraction: -
4. Division: /

The modulus operation is not in floating point math (that is int)

Remainder: %

# Short Cuts: Unary Operators

```
X+=5   short cut for x=x+5
X-=5   short cut for x=x-5
x/=5   short cut for x=x/5
x*=5   short cut for x=x*5

These do not work in floating point math (it works, but not well with doubles, so only use these for int)

x++
X-- 
```

# Craziness 

`Math.pow(double x, double y)` calculates the exponent
Try the following
* `double y = Math.pow(4,2);` = `16.0`
* `double y = Math.pow(4,0.5);` = `2.0`
* `double  y = Math.pow(4,1/2);` = `1.0`

In math, type is sensitive. `1/2` returns 0 (int division) while `1.0/2.0` returns 0.5. So what's going on?

* Integer operating on an integer results in an integer
* Double operating on an integer results in a double
* Double operating on a double results in a double

So...
* 1/2 is 0
* 1.0/2 is 0.5
* 1/2.0 is 0.5

# Typecasting

What if you have two variables dividing one another?  x/y  
You can multiply one of them by 1.0 : (1.0*x)/y   
You can also cast.  
Casting changes one form into another.  This is simple for certain cases but not for others.  
To convert an integer to a double, you do `(double) x`

So you can get (double)x/y or x/(double)y

BUT be careful of operator precedence (Order of Operations).  Just put a parenthesis around one variable to make sure
((double)x)/y

In this code snippet, something interesting happens.
```
int x=3;
int y=2;
double z;
z=(double)(x/y);
System.out.println(z);
```
The program returns `1.0`

# Floating Points Video

# == and floating point numbers

Do NOT ever use the equals (==) comparison on floating point numbers. The precision is affected, and you will possibly get a long number.

For example: You know that (4.3-2.1)/10 is 0.22 (from math).  
Doing `System.out.println((4.3-2.1)/10);` in Java returns `0.21999999999999997`, which is not equal to `0.2`

You have no idea what they really are. Use x<=c and x>=c

Do this:  `Math.abs(x-c)<r` where `r` is tolerance.

For example, if you want to see if x is equal to 3, use `Math.abs(x-3)<0.00001` and not `x == 3`
