# Spring Boot app demo on Azure

This is the implementation of [Deploy a Spring Boot app to Azure App Service](https://learn.microsoft.com/en-us/training/modules/deploy-java-spring-boot-app-service-mysql/) example
contained in  [Get started with Java on Azure](https://learn.microsoft.com/en-us/training/paths/get-started-java-azure/) microsoft learning path:
the example shows how to deploy a spring boot application on azure using the [azure-webapp-maven-plugin](https://github.com/microsoft/azure-maven-plugins/blob/develop/azure-webapp-maven-plugin/README.md).

## Prerequisite
To deploy the the application you need the following resources:

* An _Azure_ account
* A _Mysql_ resource deployed in _Azure Portal_ as described in reference documentation

## Start application on local machine

To start application on your local machine launch the following command from project root folder:

~~~bash
mvnw.cmd spring-boot:run
~~~

## Deploy application on azure

To deploy application on Azure launch the following command from project root folder:

~~~bash
mvn package com.microsoft.azure:azure-webapp-maven-plugin:2.13.0:deploy
~~~

### Other Documentation
* [Azure for developer](https://learn.microsoft.com/it-it/azure/developer/java/?WT.mc_id=java-10785-ropreddy)
