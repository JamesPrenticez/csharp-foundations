(Get the .net SDK for VSCODE)[https://dotnet.microsoft.com/en-us/download/dotnet/sdk-for-vs-code?utm_source=vs-code&amp;utm_medium=referral&amp;utm_campaign=sdk-install]

Tip: restart terminal

Check the version
```bash
  dotnet --version
```
You can use a tool like dotnet script to run C# scripts (.csx files) and also regular .cs files. First, you need to install dotnet script globally:

```bash
  dotnet tool install -g dotnet-script
```

And finally we can run our code in the terminal... slowly
```bash
  dotnet script HelloWorld.cs
```