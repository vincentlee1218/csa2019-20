# AP CS A	

01 - Introduction to Java

# Programming

Programming is the art of breaking down a complex task into a series of small commands that the computer can execute.  For example, to boil some water for coffee:

1. Got to cabinet
2. pick out kettle
3. take kettle to sink
4. turn on faucet
5. turn off faucet
6. put kettle on stove

# Java

Java comes from a language called C.  C has two visible features.

1. Each command (also called a statement) ends with a semicolon
2. You group related commands within braces

```
{
    int a=5;
    int b=7;
    int c=5+a;
}
```

can also be written like this.

`{  int a=5;int b=7;int c=5+a; }`

It is easy to understand code using indentation (four spaces). Group them with braces, finish commands with semicolons.

# Java Programs

When you write a program in java, you must create multiple files.  These are like Google Docs or Microsoft Word documents but they have these features

1. They must end in ".java"
2. They are in text format
3. You must put one class per file and it must have the same name as the name of the file.

Pikachu.java must have "class Pikachu" 

BattleArena.java must have "class Battle Arena"

# Let's write our first Java program

1. Go to [repl.it Classroom Link](https://repl.it/classroom/invite/cwGnT25)
2. Log in with Google

# In repl.it

1. You are in a file called Main.java
2. Erase everything it gives you.  We are going to write our own.
3. Because the file name is called Main.java, we must start with
4. The braces tell us that everything we write is grouped in the Main class. 
```
class Main
{
}
```
5. The word "class" is unfamiliar to most of you.  I will explain more in September.  For now just assume you are going to start every program with the word "class ….."

# Step 2 fill in the blanks.

Inside the braces, put in 4 spaces for each line.
```
class Main
{
    public static void main (String[] args)
    {
    }
}
```
We are telling the computer that we are about to give it some instructions.  And it is called main.

# Step 2
```
public static void main(String[] args)
{
}
```
You will understand what this means later when we talk about return values, static functions, access control and arguments.  For now just memorize the command.  I will not quiz you on this command because you will end up memorizing it anyway.
A good help is PSVM

# Check

You should have the command below (without understanding anything)
```
class Main
{
    public static void main(String[] args)
    {
    }
}
```
The only thing you have to know is
1. Main.java erquires class Main
2. Braces group commands.  Indent 4 spaces inside

# Step 3
```
class Main
{
    public static void main(String[] args)
    {
        System.out.println("Hello World!");
    }
}
```

# Printing

System.out.println();
1. If you need to print something, you use this command.  The quotation marks show that you are requiring exact values
2. System is a static class.
3. out is the output stream 
4. println() is a method that belongs to the out stream.
5. You should be now completely confused because you do not know what a static class, a stream or a is.  I will explain.  For now, just memorize the function.

# Review

1. Erase everything in repl.it and write it from scratch 3 times.
2. On a sheet of paper, write it once from memory.
3. I am asking you to write it on paper because I need to build your muscle memory and also to get you used to writing functions on paper.  It is an AP requirement
4. Check for proper indentations.

# Creating a variable

1. A variable in a programming language is like a storage for holding things.
2. We will practice with an int variable.
3. It holds integers
```
int a=5;
System.out.println(a);
System.out.println("a");
```
# Here is a sample program:

```
class Main {
  public static void main(String[] args) {
    System.out.println("Hello world!");
  }
}
```

Now write `public static void main(String[] args)` five times.

https://repl.it/student/classrooms/77487

https://repl.it/student/classrooms/142817

# so what's going on?

In the program we just created in Repl.it:

`class` is the class that is necessary for a program to run. The name of the class has to match with the file name, or it won't execute properly.

"Main" is the name of the file and corresponds to the file name (in this case, Main.java).

`public static` are modifiers. `public` shows that you have a public object. \
Public means that the method can be called from anywhere. Private means that the method can only be called from its own class. These two terms are used in access control. \
Static means that the method can be accessed without an instance of the class. Static methods don't need to be invoked on the object and that is when you use it. Example: your Main() is a static and you don't create an object to call it.

`void` is a return type of the method. A method must return a variable of the type that is specified. \
So if you have `public static int` for a method that method will have to return a variable of type int. \
However, `void` methods (such as the Main() method) do not return a variable in respond to its call, hence the name void.

The second `main` in this program is the method name. The main method in the file is the first method that Java will execute in a file. You can create other methods in a class (file) by creating a method, say `public static void NewMethod(args) {` and then using the call method function `NewMethod(args)`. The arguments used in a method will be described later in the text.

`String[] args` means the method accepts an array of strings. Arguments for other methods may vary and are found inside the parentheses of a method signature. \
If a method name has `(int a, double b)` in its method signature, the method takes in an integer variable a and a double variable b. \
These arguments serve another purpose: When two methods have the same name, but different sets of arguments (in type and/or order and/or number of arguments), Java can tell which method is being called. This is called overloading a static method.

Both the `class` and `void` methods have brace to enclose the groups, as you can see. Now let's take a look at the next command.

Inside the System.out.println() command, `System` is a static class that Java calls. `out` refers to the output stream in this class. `println()` is a method within the System.out class stream. What goes inside the parentheses is the contnet that has to be printed as output. This can vary from variables, to numbers, to strings, or a combination of these.

A semicolon ends the command most of the time. The combination of braces, parentheses, and semicolons allows a Java program to be written on just one line and/or without spaces or indentations. Python, however, utilizes the spacing and lines in the program to read and execute the program, so the indentations and lines are necessary in that language. 

To declare a variable, use `vartype varname = value;`. The `vartype` is the variable type, such as int or String. The `varname` can be a normal name, however it must follow some special conventions, including no spaces, cannot start with a number, and certain punctuation marks only. Remember the semicolon ends the command.

Over this course, we will go over many examples that apply these terms.

Did you know that Java compiles the program first before running it, while Python reads and executes each line separately (like an interpreter)? This is the difference between a program compiler language and an interpreter language. Compilers compile the program first and then run, while interpreters use a REPL (Read-Evaluate-Print-Loop) to execute each line individually.
