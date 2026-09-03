# CalculatorApp

1. Overview

CalculatorApp is a minimal .NET console application that demonstrates a tiny Calculator class which can add two integers. It is intended as a learning/demo project showing how to write a small class, exercise it with SpecFlow feature files (Gherkin) and run the scenarios using MSTest.

2. Description

This repository contains:
- Calculator.cs — a simple Calculator class with an Add(int a, int b) method.
- Program.cs — the console application entry point (minimal for the demo).
- Features/Calculator.feature — a SpecFlow Gherkin feature that describes the add-two-numbers scenario (5 + 3 = 8).
- Steps/CalculatorSteps..cs — SpecFlow step definitions that call Calculator.Add and assert the result with MSTest.

The project targets .NET 10.0 and uses SpecFlow with MSTest as the test runner. The project file (CalculatorApp.csproj) includes the SpecFlow MsTest packages and the Microsoft Test SDK packages required to build and run the feature-based tests.

3. Prerequisites

- .NET SDK 10.0 or later installed: https://dotnet.microsoft.com/
- A terminal / PowerShell / command prompt with `dotnet` available
- (Optional) An IDE such as Visual Studio 2022+ or Visual Studio Code with C# support for a better editing and debugging experience

4. Build and Run

From the repository root, restore packages, build the project, run the console app (demo), and run the tests:

```bash
# restore dependencies
dotnet restore

# build the project
dotnet build

# run the console application (the Program.cs in this demo project is minimal)
dotnet run --project CalculatorApp.csproj

# run tests (SpecFlow scenarios are executed by MSTest via dotnet test)
dotnet test
```

Notes

- The SpecFlow feature lives at `Features/Calculator.feature` and the step definitions are in `Steps/CalculatorSteps..cs`.
- `dotnet test` will discover and run the generated SpecFlow tests using MSTest; SpecFlow MSBuild generation is configured in the project file.
