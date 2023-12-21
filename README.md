# How to create in VSCode .NET 8 Web API and deploy it to Azure WebApp with Azure CLI

## Summary

In this example we show you how to create a new .NET 8 WebAPI and how to deploy it in Azure Web App with only two commands:

```
dotnet new webapi
```

```
az webapp up ^
--name myWebAppluiscoco19777 ^
--resource-group myRG ^
--location EastUS ^
--sku B1 ^
--os-type Windows ^
--runtime "dotnet:8"
```

## 1. Create a new .NET 8 Web API in VSCode

We create a new directory where to place the new application

We run VSCode and in a Terminal Window we run this command:

```
dotnet new webapi
```

This is by default the Web API application project folders structure

![image](https://github.com/luiscoco/Azure_WebApp_Deploy_WebAPIdotNET8_with_AzureCLI/assets/32194879/4a31fdb0-b8a7-463c-b142-d491ebae33b0)

If we would like to include some features when creating the application we can run this command to list the available application features

```
dotnet new webapi --help
```

## 2. Deploy the .NET 8 Web API in Azure Web App

With the following command automatically we create a new Azure AppService Plan and also a new Azure Web App

```
az webapp up --name myWebAppluiscoco19777 --resource-group myRG --location EastUS --sku B1 --os-type Windows --runtime "dotnet:8"
```

![image](https://github.com/luiscoco/Azure_WebApp_Deploy_WebAPIdotNET8_with_AzureCLI/assets/32194879/4043e668-fbb7-42a4-90ee-22441df6b93c)

We verify the new Web API application

![image](https://github.com/luiscoco/Azure_WebApp_Deploy_WebAPIdotNET8_with_AzureCLI/assets/32194879/250c7b85-089a-4b0b-8b01-46658ebd7fe5)




