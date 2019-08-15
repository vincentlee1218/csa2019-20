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

It is easy to understand code using identation (four spaces). Group them with braces, finish commands with semicolons.

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
System.out.println("a');
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
