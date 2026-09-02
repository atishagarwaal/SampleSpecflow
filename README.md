# CalculatorApp

A very small .NET console app that adds two numbers. The project includes a simple Calculator class and tests written with SpecFlow and MSTest.

## What it does
- Adds two numbers using Calculator.Add(a, b).
- Tests the addition with a Gherkin scenario: 5 + 3 = 8.

## Files you should know
- `Calculator.cs` - contains the Calculator class with the Add method.
- `Program.cs` - the app entry (minimal).
- `Features/Calculator.feature` - SpecFlow feature (Gherkin) that describes the test scenario.
- `Steps/CalculatorSteps..cs` - step definitions that run the scenario and call the Calculator.

## How to build and run tests
1. Make sure you have the .NET SDK installed: https://dotnet.microsoft.com/download
2. In the repo folder, run:

```bash
dotnet build
dotnet test
```

The tests use SpecFlow and MSTest. No special setup or secrets are needed.

## Add more tests
- To add more examples, edit `Features/Calculator.feature` and add new scenarios.
- Implement any new steps or logic in `Steps/CalculatorSteps..cs` and `Calculator.cs`.

## Notes
- This is a tiny demo project meant for learning how to use SpecFlow with MSTest.
