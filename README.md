# Provider Service API - Unit Tests

## Description

This project contains unit tests for the **Provider Service API** developed in .NET 6. NUnit is used to perform tests on the controllers, ensuring that the API functions correctly and meets the requirements.

## Technologies

- .NET 6
- NUnit (for testing)
- Moq (for dependency mocking)

## Installation

1. **Clone the repository**:

   If you already have the main project repository cloned, the testing project will be inside it. If not, clone the repository:

   ```bash
   git clone https://github.com/your-username/ProviderServiceAPI.Tests.git 

2. Restore NuGet packages:

From the command line or Visual Studio, run the following command to restore the necessary packages:

dotnet restore

3. Run tests:

To run the unit tests, you can use either Visual Studio or the command line. Here's how to do it:

Using Visual Studio
Open the project solution in Visual Studio.
Go to the Test Explorer window (Ctrl+E, T).
Click "Run All Tests" to execute the tests.
Using the Command Line
From the root of the test project, run:

dotnet test

This will execute all the tests in the project and display the results in the terminal.

4. Covered Tests
Authentication
Login with valid credentials: Verifies that the authentication controller returns a JWT token when the user provides valid credentials.
Login with invalid credentials: Verifies that the authentication controller returns Unauthorized when the user provides invalid credentials.
Provider Management
Create a provider: Verifies that the provider controller correctly creates a provider and returns a CreatedAtActionResult.
Get all providers: Verifies that the controller returns a list of providers.
5. Mocking
The project uses Moq to mock dependencies such as IUserRepository and IProviderRepository, allowing isolated unit testing without interacting with the database.
