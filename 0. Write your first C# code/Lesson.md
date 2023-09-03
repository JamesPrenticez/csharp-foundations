# Write your first line of C# code

```cs
  Console.WriteLine("Hello World!");
```

The green Run button performs two tasks:

It compiles your code into an executable format that a computer can understand.
It runs your compiled application and, when written correctly, will output "Hello World!".


Writing C# code is an exercise in precision. If you type just one character incorrectly, you'll get an error message

for example a lowercase "c" would an error
or if you used single-quotation marks (') to surround the literal string Hello World!

```cs
  console.WriteLine("Hello World!");
  Console.WriteLine('Hello World!');
```

```error
  (1,1): error CS0103: The name 'console' does not exist in the current context
  (1,19): error CS1012: Too many characters in character literal
```
The first part (1,1) indicates the line and column where the error occurred

Comments are nice 
```cs
// Console.WriteLine("Hello World!");
```

# The difference between Console.Write and Console.WriteLine

Write everything on a **new** line
```cs 
  Console.WriteLine("Hello World!");
```

Writes everything on **one** line or **paragraph**
```cs
  Console.Write("Congratulations!");
  Console.Write(" ");
  Console.Write("You wrote your first lines of code.");
```

# Learn how it works

A special program called a compiler converts your source code into a different format that the computer's central processing unit (CPU) can execute.

The Console part is called a class. 
Classes "own" methods;
The parentheses are known as the method invocation operator.

Finally, the semicolon is the end of statement operator. A statement is a complete instruction in C#. The semicolon tells the compiler that you've finished entering the command.

