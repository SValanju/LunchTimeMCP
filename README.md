# LunchTimeMCP

LunchTimeMCP is a .NET 9 server application designed to help teams decide where to go for lunch. It allows users to add restaurants, view available options, pick a random restaurant, and track visit statistics.

## Features
- Add new restaurants with cuisine type and location
- List all available restaurants
- Pick a random restaurant for lunch
- View visit statistics for each restaurant

## Prerequisites
- [.NET 9 SDK](https://dotnet.microsoft.com/en-us/download/dotnet/9.0)
- [ModelContextProtocol --prerelease](https://www.nuget.org/packages/ModelContextProtocol) (NuGet package)
- [Microsoft.Extensions.Hosting](https://www.nuget.org/packages/Microsoft.Extensions.Hosting) (NuGet package)

## Configuration & Setup

1. **Clone the repository**
   ```sh
   git clone <repository-url>
   cd LunchTimeMCP
   ```

2. **Restore dependencies**
   ```sh
   dotnet restore
   ```

3. **Build the project**
   ```sh
   dotnet build --configuration Release
   ```

## Using with GitHub Copilot Agent Mode

To use this MCP app in GitHub Copilot agent mode:
1. Ensure the `.mcp.json` file is present in the root folder of your project. This file configures the MCP server for Copilot agent integration.
2. Open GitHub Copilot chat in your development environment.
3. Switch to Agent Mode in Copilot chat.
4. In the tools section, select your project name (e.g., LunchTimeMCP) to connect the agent to your MCP server.
6. Ask the Copilot agent to perform actions like adding restaurants, listing options, or picking a random restaurant.

Refer to the Copilot agent documentation for details on agent mode setup and integration.

## Using with ModelContextProtocol/Inspector

To use LunchTimeMCP with ModelContextProtocol/Inspector:

### 1. Install Inspector
Install the Inspector tool (refer to the official documentation for platform-specific instructions). Available as a node package, use:
```sh
npm install -g @modelcontextprotocol/inspector
```

### 2. Launch Inspector
Start the Inspector tool by running:
```sh
npx @modelcontextprotocol/inspector dotnet run
```

### 3. Use Inspector
- Once the Inspector is running, it will provide an interactive interface.
- Click on Connect to start a session with the MCP server.
- Once connected, you can interact with the MCP server using the Inspector's UI.

Refer to the [Inspector](https://modelcontextprotocol.io/legacy/tools/inspector) documentation for advanced usage and troubleshooting.
