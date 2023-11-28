# Install and Configure Visual Studio Code

**IMPORTANT**
you need to cd into the project or VScode get all confused

.NET CLI command will create a new console application in the specified folder location

[https://learn.microsoft.com/en-us/training/modules/install-configure-visual-studio-code/7-exercise-create-build-run-app]

```cs
dotnet new console -o ./CsharpProjects/TestProject
```

# Call Methods From the .NET Class Library Using csharp
```cs
Random dice = new Random();
int roll = dice.Next(1, 7);
Console.WriteLine(roll);
```

**Stateful versus stateless METHODS**
STATEFUL (instance) = In software development projects, the term state is used to describe the condition of the execution environment at a specific moment in time.
As your code executes line by line, values are stored in variables. At any moment during execution, the current state of the application is the collection of all values stored in memory. They're also known as **instance methods**.

STATELESS (static) = methods are implemented so that they can work without referencing or changing any values already stored in memory. Stateless methods are also known as static methods. 

For example, the Console.WriteLine() method doesn't rely on any values stored in memory. It performs its function and finishes without impacting the state of the application in any way.

Other methods, however, must have access to the state of the application to work properly. In other words, stateful methods are built in such a way that they rely on values stored in memory by previous lines of code that have already been executed.

When you need to call stateful methods, you must first create an instance of the class so that the method can access state.

# Creating an instand of a class (instantiate)
The new operator does several important things:

1. It first requests an address in the computer's memory large enough to store a new object based on the Random class.
2. It creates the new object, and stores it at the memory address.
3. It returns the memory address so that it can be saved in the dice variable.

**WOW - how random works**
To create the illusion of randomness, the developers of the Next() method decided to capture the date and time down to the fraction of a millisecond and use that to seed an algorithm that produces a different number each time.

# How can you determine whether you need to create an instance of a class before calling its methods?

1. Doumentation [https://learn.microsoft.com/en-us/dotnet/api/system.random.next?view=net-8.0]
2. Let VSCode tell you off

# Exercise - Return values and input parameters of methods
### Return values
Some methods are designed to complete their function and end "quietly". In other words, they don't return a value when they finish. They are referred to as void methods.

Other methods are designed to return a value upon completion. The return value is typically the result of an operation. A return value is the primary way for a method to communicate back to the code that calls the method.

### Overloaded methods
Many methods in the .NET Class Library have overloaded method signatures. Among other things, this enables you to call the method with or without parameters.

An overloaded method is defined with multiple method signatures. Overloaded methods provide different ways to call the method or provide different types of data.
