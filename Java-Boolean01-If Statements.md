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

>   Greater than    \
>=  Greater than or equal   \
<   Less than   \
<=  Less than or equal  \
==  Equals to   \
!=  Not equals to   \

# Let's try input
```
import java.util.Scanner;
class Main{
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

Decimal Numbers work like Integers but do NOT USE \
==    because decimal numbers are guaranteed to have rounding errors \
Instead use
```
abs(a-b)<tolerance
abs(x-3.14)<0.01
```

# Boolean Variables

Sometimes you want to use a variable that is a Boolean.  Then call the variable \
isSomething or  (`isDog, isBoy, isSpanishSpeaking`) \
hasSomething (`hasDegree, hasCar, hasLicense`) \
Then do \
`if (isSpanishSpeaking)` and not `if(isSpanishSpeaking==true)` \
or `if (!isSpanishSpeaking)`

# classes

Objects do not use == \
Objects use the .equals() method.   \
I will explain later.

# Boolean Logic

NOT \
AND \
OR  \
De Morgan's Rules \

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
