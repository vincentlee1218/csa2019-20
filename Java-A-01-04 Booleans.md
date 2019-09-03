# AP Computer Science A

## 1.4 BOOLEAN

# Agenda 

1. `boolean` keyword and variables
2. The `not, or, and` operators
3. Short circuit operations (AP Topic)
4. De Morgan’s Laws (AP Topic)

# Homework

1. Complete worksheet
2. codingbat.com
   * Logic-1: cigarParty, dateFashion, squirrelPlay, caughtSpeeding, sortasum (first 5)

# Boolean

One of three primitives you need to know for AP CS A,  
`boolean` takes on two values only : true and false.

The result of tests can also be a boolean value and can be assigned to a variable
```
    if (x==2) {
       isEqual==true;
    }
        boolean isEqual = (x==2);
```

# Declaring Boolean variables

You can explicitly create a Boolean variable
```
boolean isRaining;
isRaining=true;

boolean isRaining=false;
```

The result of a Test can be a Boolean.  In this case you do not have to declare a variable

`(3<=5)`: results in true

`(5<3)` : results in false

# Using Booleans to make decisions

Use Booleans as “flags” to store state make decisions.
```
if (hasSword)
{     
   System.out.println(“Attack!”);
} else
{
   System.out.println(“Retreat!”);
}
```

Tests : Use to compare
```
if (x>5)
{     
   System.out.println(“Big”);
} else
{
   System.out.println(“Not”);
}
```

# Boolean Operators

You can use Boolean operators to create complex expressions. There are three Boolean operators you need to know.

1. OR   ||
2. AND &&
3. NOT  !

# The not keyword:  !

The not operator is used to negate an expression, or to turn it into its opposite
For example, `!true` would evaluate to `false`, and `!false` would evaluate to `true`

`(!isHot)` is the same is `(isHot==false)`
`(a!=10)` is the same is `!(a==10)`

# The and keyword:  &&

The `&&` keyword is used when two elements must both evaluate to `true` in order for the overall Boolean expression to be `true`

The general formula is: `<boolean expression> && <boolean expression>`
```
if (2 + 2 == 4 && 1 + 1 == 2) {
	System.out.println(“Both operations are true”);
}
```

# The or keyword:  ||

`or` is used when only one of the two elements must evaluate to true in order for the overall boolean expression to be `true`.  If both elements are true, it will also evaluate to `true`.
The general formula is: `<boolean expression> || <boolean expression>`
```
int count = 10;

if (count == 10 || false) {
	System.out.println(“One of the expressions is true”);
}
```

# Order of Operations

1. NOT is executed first
2. AND is executed second
3. OR is executed last

```
int x = 4, y = 5, z = -20;
if (x == 4 || y > 7 && !(z < -10) )
{
    System.out.println ("Something prints");
}
```

If you want the || before the &&, put them in parenthesis
```
if ((x == 4 || y > 7) && !(z < -10) )
{
    System.out.println ("Something prints");
}
```

# Short Circuit Operations

In Java, the Boolean operators (&& and ||) are short-Circuit operators.
```
if (A||B){}
if (A&&B){}
```
After these operators get the result of A, they will evaluate B only if necessary.

# OR Operator

Let’s consider
```
if (A||B)
{
    System.out.println(“OR”);
}
```

```
A    B    A||B
T    T    T
T    F    T
F    T    T
F    F    F
```

You can see from the truth table that if A is `true`, the expression is `true` no matter what value B is.

So Java will not test B. If B has an error, it is not detected.

# AND  Operator

Let’s consider
```
if (A&&B)
{
    System.out.println(“AND”);
}
```
```
A    B    A||B
T    T    T
T    F    F
F    T    F
F    F    F
```

You can see from the truth table that if A is `false`, the expression is `false` no matter what value B is.

So if A is `false`, Java will not test B. If B has an error, it is not detected.

# Example of short circuiting

## OR: If A is true, skip B

`if ( (5>3)||(5/0>6))  {}`

In this case, (5>3) is true so (5/0) is not evaluated and the error slips through

`if ( (5<3)||(5/0>6))  {}`

In this case, (5<3) is false.  Java has to test (5/3<0)  and it will catch the error.

## AND : If A is false, skip B

`if ( (5>3)&&(5/0>6))  {}`

In this case, (5>3) is true so Java will continue to evaluate (5/0).  The error is caught and will result in an error. 

`if ( (5<3)&&(5/0>6))  {}`

In this case, (5<3) is false.  Java skips (5/0) and the error is not caught.

# De Morgan Laws

De Morgan’s Laws are the “distributed property” of NOT operations.  When you distribute the ! Operator, OR becomes AND and AND becomes OR.

1. `!(a||b) = !a&&!b`
2. `!(a&&b) = !a||!b`

# Opposite of comparison operators

< is the opposite of >=

\> is the opposite of <=

== is the opposite of !=

1. `!(x <= 5)` becomes `(x > 5)`
2. `!(x == 12)` becomes `(x != 12)`
3. `!(x > 5 && y <= 2)` becomes `(x <= 5 || y > 2)`

# De Morgan’s Law Examples

1. `!(a||!b)` is also `!a && !!b` which is also `!a&&b`
2. `a&&!b` is also `!(!a || !!b)` which is also `!(!a||b)`
3. `!(a>2 || b<= 3)` is also `!(a>2)&&! (b<=3)` which is also `(a<=2 && b>3)` 
