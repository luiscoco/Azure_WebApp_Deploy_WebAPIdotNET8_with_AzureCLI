# How to create in VSCode .NET 8 Web API and deploy it to Azure WebApp with Azure CLI

## 1. Create a new .NET 8 Web API in VSCode

We create a new directory where to place the new application

We run VSCode and in a Terminal Window we run this command:

```
dotnet new webapi
```

If we would like to include some features when creating the application we can run this command to list the available application features

```
dotnet new webapi --help
```

## 2. Deploy the .NET 8 Web API in Azure Web App

With the following command automatically we create a new Azure AppService Plan and also a new Azure Web App

```
az webapp up --name myWebAppluiscoco19777 --resource-group myRG --location EastUS --sku B1 --os-type Windows --runtime "dotnet:8"
```



