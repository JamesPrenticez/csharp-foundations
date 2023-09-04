# Store and Retrieve Data Using Literal and Variable Values in C#
[https://learn.microsoft.com/en-us/training/modules/csharp-literals-variables/]

# String literal values
A literal value is a constant value that never changes.

If you write this you dont get errors?
```cs
Console.WriteLine('b');
```

but if you write this you do?
```cs
Console.WriteLine('Hello World!');
```

When you use single quotation marks, the C# compiler expects a single character

# Integer literals a numeric whole number (no fractions)

```cs
Console.WriteLine(123);
```

# Floating-point literals
C# supports three data types to represent decimal numbers: float, double, and decimal.
The compiler defaults to a double literal when a decimal number is entered without a literal suffix.

Float Type    Precision
----------------------------
float         ~6-9 digits
double        ~15-17 digits
decimal        28-29 digits

### Float
```cs
Console.WriteLine(0.25F);
```
### Double
```cs
Console.WriteLine(2.625);
```
### Decimal
```cs
Console.WriteLine(12.39816m);
OR
Console.WriteLine(12.39816M);
```

# Boolean literals

```cs
Console.WriteLine(true);
Console.WriteLine(false);
```

# Why emphasize data types?
Data types play a central role in C#. In fact, the emphasis on data types is one of the key distinguishing features of C# compared to other languages like JavaScript. The designers of C# believed they can help developers avoid common software bugs by enforcing data types. 

# What is a variable?
Variables are temporary values you store in the computer's memory

- Variable names can contain alphanumeric characters and the underscore character. Special characters like the hash symbol # (also known as the number symbol or pound symbol) or dollar symbol $ are not allowed.
- Variable names **must begin with an alphabetical letter or an underscore, not a number**.
- Variable names are case-sensitive, meaning that string Value; and string value; are two different variables.
- Variable names must not be a C# keyword. For example, you cannot use the following variable declarations: decimal decimal; or string string;.

- Variable names should use **camelCase**, which is a style of writing that uses a lower-case letter at the beginning of the first word and an upper-case letter at the beginning of each subsequent word. For example, string thisIsCamelCase;.
- Variable names should begin with an alphabetical letter. Developers use the underscore for a special purpose, so try to not use that for now.
- Variable names should be descriptive and meaningful in your app. Choose a name for your variable that represents the kind of data it will hold.
- Variable names should be one or more entire words appended together. Don't use contractions or abbreviations because the name of the variable (and therefore, its purpose) may be unclear - to others who are reading your code.
- Variable names shouldn't include the data type of the variable. You might see some advice to use a style like string strValue;. That advice is no longer current.


#  Setting and getting values from variables

```cs
string firstName;
firstName = "Bob";
Console.WriteLine(firstName);
firstName = "Liem";
Console.WriteLine(firstName);
firstName = "Isabella";
Console.WriteLine(firstName);
firstName = "Yasmin";
Console.WriteLine(firstName);
```

In fact, you can perform both the declaration and setting the value of the variable in one line of code. This technique is called initializing the variable.
```cs
string firstName = "Bob";
Console.WriteLine(firstName);
```

# Declare implicitly typed local variables
An implicitly typed local variable is created by using the var keyword
In this example, a string variable was created using the var keyword instead of the string keyword.

```cs
var message = "Hello world!";
```

In fact, the message variable is typed to be a string and can never be changed. For example, consider the following code:

```cs
var message = "Hello World!";
message = 10.703m;
(2,11): error CS0029: Cannot implicitly convert type 'decimal' to 'string'
```

If you try to use the var keyword without initializing the variable, you'll receive an error 
```cs
var message;
(1,5): error CS0818: Implicitly-typed variables must be initialized
```

```cs
string firstName;
```
