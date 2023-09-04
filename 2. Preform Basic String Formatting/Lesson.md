# Perform basic string formatting in C#
[https://learn.microsoft.com/en-us/training/modules/csharp-basic-formatting/]

# Character escape
"\" will escape a char 
"\n" will add a new line
"\t" will add a tab.
to handle that situation, use the \" escape sequence:
the \\ to display a single backslash.

```cs 
Console.WriteLine("Hello\nWorld!");
Console.WriteLine("Hello\tWorld!");
Console.WriteLine("Hello \"World\"!");
Console.WriteLine("c:\\source\\repos");
```

# Verbatim string literal
A verbatim string literal will keep all whitespace and characters without the need to escape the backslash. To create a verbatim string, use the @ directive before the literal string.

```cs
Console.WriteLine(@"    c:\source\repos    
        (this is where your code goes)");
```

# Unicode escape characters

```cs
// Kon'nichiwa World
 Console.WriteLine("\u3053\u3093\u306B\u3061\u306F World!");
```

# Cavets
There are several caveats here. First, some consoles like the Windows Command Prompt will not display all Unicode characters. It will replace those characters with question mark characters instead. Also, the examples used here are UTF-16. Some characters require UTF-32 and therefore require a different escape sequence. This is a complicated subject, and this module is only aiming at showing you what is possible. Depending on your need, you may need to spend quite a bit of time learning and working with Unicode characters in your applications

# String Concatenation

```cs
string firstName = "Bob";
string message = "Hello " + firstName;
Console.WriteLine(message);
```

# String Interpolation
```cs
string message = $"{greeting} {firstName}!";
```

```cs
string projectName = "First-Project";
Console.WriteLine($@"C:\Output\{projectName}\Data");
```

# Challenge

```cs
string projectName = "ACME";

string russianMessage = "\u041f\u043e\u0441\u043c\u043e\u0442\u0440\u0435\u0442\u044c \u0440\u0443\u0441\u0441\u043a\u0438\u0439 \u0432\u044b\u0432\u043e\u0434";

Console.WriteLine($"Veiw English output: \n\t C:\\Exercise\\{projectName}\\data.txt");
Console.WriteLine($"{russianMessage}: \n\t C:\\Exercise\\{projectName}\\ru-RU\\data.txt");

```