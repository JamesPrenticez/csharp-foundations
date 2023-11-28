#  Perform basic operations on numbers in C# 
[https://learn.microsoft.com/en-us/training/modules/csharp-basic-operations/1-introduction]

You'll use the addition operator, which is the plus symbol +. Yes, the same plus symbol + that you use for string concatenation is also used for addition

```cs
int firstNumber = 12;
int secondNumber = 7;
Console.WriteLine(firstNumber + secondNumber);
```

```cs
string firstName = "Bob";
int widgetsSold = 7;
Console.WriteLine(firstName + " sold " + widgetsSold + " widgets.");
```

Here is gets a bit funky
```cs
string firstName = "Bob";
int widgetsSold = 7;
Console.WriteLine(firstName + " sold " + widgetsSold + 7 + " widgets.");

// Bob sold 77 widgets.

// Fix it by adding parentheses ()
Console.WriteLine(firstName + " sold " + (widgetsSold + 7) + " widgets.");

// Bob sold 14 widgets.
```

```cs
int sum = 7 + 5;
int difference = 7 - 5;
int product = 7 * 5;
int quotient = 7 / 5;

Console.WriteLine("Sum: " + sum);
Console.WriteLine("Difference: " + difference);
Console.WriteLine("Product: " + product);
Console.WriteLine("Quotient: " + quotient);

// Sum: 12
// Difference: 2
// Product: 35
// Quotient: 1 ?? no remainder

decimal decimalQuotient = 7.0m / 5;
Console.WriteLine($"Decimal quotient: {decimalQuotient}");

// Decimal quotient: 1.4
```

**Perform a data type cast from int to decimal**

```cs
int first = 7;
int second = 5;
decimal quotient = (decimal)first / (decimal)second;
Console.WriteLine(quotient);

// 1.4
```

The modulus operator % tells you the remainder of int division.
```cs
Console.WriteLine($"Modulus of 7 / 5 = {7 % 5}");

// 
```

Challenge -  Calculate Celsius given the current temperature in Fahrenheit

```cs
int f = 94;

var res = (94 - 32m) *  (5m/9m);;
Console.WriteLine(res);
```
