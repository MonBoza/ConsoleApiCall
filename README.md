## Get Developer API Key

This project uses the New York Times' Top Stories API to practice making API calls in C#. In order to use the Top Stories API, you'll need to create a free New York Times developer account. Follow the Get Started steps to create an application and get your own API key.

### Set Up and Run Project - Branches 1 and 2 Only

The following setup instructions are for the branches 1_api_call_in_console_app and 2_deserializing_responses_in_console_app only.

#### Clone this repo.

Open the terminal and navigate to this project's production directory. called "ConsoleApiCall".
Within the production directory "ConsoleApiCall", create a new file called EnvironmentVariables.cs.
Within EnvironmentVariables.cs, put in the following code, replacing the [YOUR-API-KEY-HERE] with your own New York Times API key.

```
namespace ConsoleApiCall.Keys
{
  public static class EnvironmentVariables
  {
    public static string ApiKey = "[YOUR-API-KEY-HERE]";
  }
}
```

Within the production directory "ConsoleApiCall", run dotnet run in the command line to start the project in development mode with a watcher.
Set Up and Run Project - Branch 3 Only
The following setup instructions are for the branch 3_api_call_in_mvc_app only.

Clone this repo.
Open the terminal and navigate to this project's production directory. called "MvcApiCall".
Within the production directory "MvcApiCall", create a new file called appsettings.json.
Within appsettings.json, put in the following code, replacing the [YOUR-KEY-HERE] with your own New York Times API key.

```
{
  "NYT": "[YOUR-KEY-HERE]"
}
```

Within the production directory "MvcApiCall", run dotnet watch run in the command line to start the project in development mode with a watcher.
Open the browser to https://localhost:5001. If you cannot access localhost:5001 it is likely because you have not configured a .NET developer security certificate for HTTPS. To learn about this, review this lesson: Redirecting to HTTPS and Issuing a Security Certificate.