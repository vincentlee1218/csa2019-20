# AP Computer Science A

## 1.1 Primitive Data Types

# Variables

* Computers work with data by storing it in memory.   
* Computer memory is very big, so it is divided up into pieces, and each piece has an address.
* Data stored in the computer's memory is referred to by a reference to that memory location called a variable.
* Variables work like variables in math: they can hold date that change.  But they are references to memory locations in human friendly format.

# Variable Types

* Computers store data in different formats.
* Counting numbers are stored in binary (1=00000001, 2=00000010)
* Rational Numbers (decimals) are stored in "scientific notation" form with a mantissa and an exponent. (30.2 = 3.02 x 10^2)
* Characters are stored in a code (A=65, B=66, ...)
* When you create a variable, you need to specify what the type of data it is so the computer store and use them correctly.

# Primitives: You must know these!

## MUST know (quiz)

* int : integers.  Positive, negative.  No decimals.  Example: 3, -5, 126, 0
* double : real numbers.  Positive, negative, decimals. Example 3.14, 9, 0, 42.
* boolean :  true or false

## Helpful to know

* char.  A single alphanumeric character.  For example, “a”.
* "4" is different from 4.  4 is a number.  "4" is a character.  4+5=9.  But "4"+"5"="45".

# Declaring variables.

* If you want to store a value in a variable, you have to first tell Java what kind of value will be stored in that variable. 
* This is called a declaration, which is often at the beginning of a section of code.
* So to store the value 13 in a variable called `luckyNumber`, you first have to declare the variable and the type of data that you'll be storing in it:
* `int luckyNumber; // declare that luckyNumber will be "storing" an integer`
# Assigning Values to variables

* Once you've established a variable, you can then use the assignment operator to identify the primitive or object that the variable will refer to
* This is the assignment operator.  In Java this is the equals sign = to identify the primitive or object that the variable will refer to. 
* The value on the right becomes associated with the identifier on the left. (It is not a statement of equality like it is in math.)

# Assigning new values to a variable

* If you want to change the value that a variable refers to, use the equals sign again:
* `luckyNumber = 12;     // variable is already declared, don't need to do it again!`
* Whatever value was stored in `luckyNumber` before is no longer available to us. We have overwritten its value with this new, updated value.

# Assigning during declarations

```
int  luckyNumber;
luckyNumber = 13;
```

`int luckyNumber=13;`

# (Rule) What can you use in your variable names?

* Can be made of letters, numbers, $, and _, but can't begin with a number
* Can't have special characters like !, #, or spaces
* Can’t be reserved words that have special meaning in Java (`public, class, main, etc.`)
* Are case-sensitive

# Conventions

* Variable and method names begin with a lower-case letter.  Example `laserDamage, shieldStrength`.
* Class names (we'll learn about classes soon) begin with an upper case letter.  Example: `Pokemon, Student, Automobile`
* No underscores in identifiers—use camelCase for multi-word variables
  * Prefer:       `laserDamage`
  * Avoid:        `laser_Damage   (this is from C/C++)`

# Scope!!!!!!!!

* Variables are valid within the {} in which they are created.
```
{
    int   numberOfBurgers=10;
    numberOfBurgers=12;

    {
        numberOfBurgers=300;
    }
}
```
**numberOfBurgers=2000;   // INVALID.  Outside of {}**

# Data Types in Java (AP CS A)

* There are three java data types you muse be familiar with
  1. Primitives : Holds a single piece of information : A number, a character,  a true/false value
  2. An Array or List : Holds a lot of information of a single type
  3. An Object : Holds a mixture of data types and functions to modify them.
