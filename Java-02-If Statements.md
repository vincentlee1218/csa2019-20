# If Statements

Boolean Logic 1

# Use an If statement

```
if (true)
{
    System.out.println("So True");
} else
{
    System.out.println("Not Really");
}
```

# Let's Find a statement that is true

```
if (5>3)
{
    System.out.println("So True");
} else
{
    System.out.println("Not Really");
}
```

# Let's use variables

```
int a=5;
int b=3;

if (a>b)
{
    Sop("So True");
} else
{
Sop("Not Really");
}
```

# Integer Operations that return true/false

>   Greater than  
>=  Greater than or equal  
<   Less than  
<=  Less than or equal  
==  Equals to  
!=  Not equals to  

# Let's try input
```
import java.util.Scanner;
class Zion{
    psvm{
        Sop("Type in a number");
        Scanner  s = new Scanner(System.in);
        int n = s.nextInt();
        if (n%2==0)
            Sop("Is Even");
        else
            Sop("Is Odd");
    }
}
```
# Let's what those braces do

```
if (true)
{
    Sop("One");
    Sop("Two");
    Sop("Three");
    Sop("Four");
}
```

```
if (true)
{
    Sop("One");
    Sop("Two");
}
Sop("Three");
Sop("Four");
```

```
if (true)
{
    Sop("One");
    Sop("Two");
} else
{
    Sop("Three");
    Sop("Four");
}
Sop("Five");
Sop("Six");
```

# Decimal Numbers DON'T a==b

Decimal Numbers work like Integers but do NOT USE  
==    because decimal numbers are guaranteed to have rounding errors  
Instead use
```
abs(a-b)<tolerance
abs(x-3.14)<0.01
```

# Boolean Variables

Sometimes you want to use a variable that is a Boolean.  Then call the variable  
isSomething or  (`isDog, isBoy, isSpanishSpeaking`)  
hasSomething (`hasDegree, hasCar, hasLicense`)  
Then do  
`if (isSpanishSpeaking)` and not `if(isSpanishSpeaking==true)`  
or `if (!isSpanishSpeaking)`

# classes

Objects do not use ==  
Objects use the .equals() method.  
I will explain later.

# Boolean Logic

Boolean logic is named after George Boole and is the foundation of modern computers.

It is based on **true** or **false** values of variables.

Computers are binary 0 or 1.  0 is associated with false and 1 is associated with true.

Boolean logic is associated with

1. Logic statements and decisions
2. Binary switching
3. Calculating

# Boolean Variables

A boolean variable only has two values.  "true" and "false"
```
boolean isHungry;
if (isHungry==true)
    doSomething
else
   doAnotherTHing

if (isHungry)
    doSomething
else
   doAnotherThing
```

States of isHungry

isHungry    true    false

# Boolean Logic NOT

! is NOT.  It is associated with the Opposite.  
It can check for false.  It can change the state.

## Flip a value
```
boolean isHungry=true;
isHungry = !isHungry
```
## Check
```
if (!isHungry)
    doSomething

```
## Warning 
x!=y        means not equals to
y=!x        means assign y opposite of x
```
isFed   T   F  
!isFed  F   T
```
# Boolean Logic AND

AND is an operator.

It takes two variables and returns a value.

It is associated with Multiplying.

It returns true if and only of both A and B are true.
```
X       Y       X AND Y
true    true    true  
false   true    false  
true    false   false  
false   false   false  
```
# Boolean Logic OR

OR is an operator.

It takes two variables and returns a value.

It is associated with Adding.

It returns true if any variable is true
```
X       Y       X OR Y  
true    true    true  
false   true    true  
true    false   true  
false   false   false  
```
# Boolean Logic

De Morgan's Rules

NOT(A OR B) = NOT(A) AND NOT(B)

NOT(A AND B) = NOT(A) OR NOT(B)

# Exercises

1. Ask for a number.  If it is divisible by 4 type "Quads",  if it is divisible by 2 but not by 4 type "Doubles", if it is an odd number, type "ODDS"
2. Ask for a number, if it is divisible by 2, type "Doubles", if it is divisible by 3, type "Trios", if it is divisible by both 2 and 3 (or divisible by 6), type "Both".  If it is not divisible by any of these, type "NONE"
3. Ask for a number.  If it is divisible by 2 type "DOUBLE", if it is divisible by by 5, type "Penta", if it is divisible by neither or divisible by both type "NONE".
4. Ask for a number.  If it is divisible by by 3 but not by 9 type "Trio".  If it is divisible by 9,type  "Lose:", if it is not divisible by 3, type "Pass"

# Boolean logic vs nested

`if (A AND B)`

```
if (A)
    if (B)
```

# Nested If statements

```
if {}
else if {}
else {}

if{
    if{} else{}
}
else {}
```
