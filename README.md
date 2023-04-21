# funapp-hello-world

This is a basic Azure function app displaying "Hello World" when called.

[This](https://learn.microsoft.com/en-us/azure/azure-functions/create-first-function-cli-csharp?tabs=azure-cli%2Cin-process) guide can be followed to create and configure a new function app.

## How to run

Start up the function app by running the following command in the root directory of the project:

```bash
func start
```

## How to deploy

Deploy the function app to Azure by running the following command in the root directory of the project:

```bash
func azure functionapp publish <function-app-name>
```

## How to call

Call the function app by starting up the function app and running the following command, or pasting the URL in your browser:

Local version

```bash
curl http://localhost:7071/api/HelloWorld
```

Deployed version

```bash
curl https://<function-app-name>.azurewebsites.net/api/HelloWorld
```

## How to test

Test the function app by running the following command in the root directory of the project:

```bash
func azure functionapp fetch-app-settings <function-app-name>
func host start
```

## How to debug

Debug the function app by running the following command in the root directory of the project:

```bash
func azure functionapp fetch-app-settings <function-app-name>
func host start --debug vscode
```

## How to build

Build the function app by running the following command in the root directory of the project:

```bash
func azure functionapp publish <function-app-name> --build-native-deps
```

## How to create

A function app can be created using the following command in the root directory of the project:

```bash
func init <function-app-name>
```

## How to create a new function

Create a new function by running the following command in the root directory of the project:

```bash
func new
```

## How to create a new function with a specific language

Create a new function by running the following command in the root directory of the project:

```bash
func new --language <language>
```

## How to create a new function with a specific template

Create a new function by running the following command in the root directory of the project:

```bash
func new --template <template>
```
