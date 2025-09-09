[...existing code...]
# Library App

## Description

Library App is a modular C# solution for managing library operations. It is organized into core, infrastructure, and console projects, with unit tests for validation. The application demonstrates clean architecture principles, separation of concerns, and extensibility for future features.

## Project Structure

- AccelerateDevGitHubCopilot.sln
- README.md
- src/
	- Library.ApplicationCore/
		- Library.ApplicationCore.csproj
		- Entities/
		- Enums/
		- Interfaces/
		- Services/
	- Library.Console/
		- appSettings.json
		- CommonActions.cs
		- ConsoleApp.cs
		- ConsoleState.cs
		- Library.Console.csproj
		- Program.cs
		- Json/
	- Library.Infrastructure/
		- Library.Infrastructure.csproj
		- Data/
- tests/
	- UnitTests/
		- LoanFactory.cs
		- ...

## Key Classes and Interfaces

- **Entities/**  
	Domain models representing core library concepts (e.g., books, loans, users).

- **Enums/**  
	Enumerations for domain-specific states and types.

- **Interfaces/**  
	Abstractions for services and repositories, enabling dependency injection and testing.

- **Services/**  
	Business logic implementations for library operations.

- **Library.Console/Program.cs**  
	Entry point for the console application.

- **Library.Console/CommonActions.cs**  
	Shared actions and utilities for console workflows.

- **Library.Infrastructure/Data/**  
	Data access and persistence logic.

- **tests/UnitTests/**  
	Unit tests for validating core logic and behaviors.

## Usage

1. **Build the Solution**  
	 Open the solution in Visual Studio or run:
	 ```sh
	 dotnet build
	 ```

2. **Run the Console Application**  
	 ```sh
	 dotnet run --project src/Library.Console/Library.Console.csproj
	 ```

3. **Execute Unit Tests**  
	 ```sh
	 dotnet test tests/UnitTests/UnitTests.csproj
	 ```

## License

This project is licensed under the MIT License.
Coming Soon
