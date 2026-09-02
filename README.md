# CalculatorApp

A very small .NET console app that adds two numbers. The project includes a simple Calculator class and tests written with SpecFlow and MSTest.

## What it does
- Adds two numbers using Calculator.Add(a, b).
- Tests the addition with a Gherkin scenario: 5 + 3 = 8.

## Files you should know
- `Calculator.cs` - contains the Calculator class with the Add method.
- `Program.cs` - the app entry.
- `Features/Calculator.feature` - SpecFlow feature (Gherkin) that describes the test scenario.
- `Steps/CalculatorSteps..cs` - step definitions that run the scenario and call the Calculator.

## Notes
- This is a tiny demo project meant for learning how to use SpecFlow with MSTest.
