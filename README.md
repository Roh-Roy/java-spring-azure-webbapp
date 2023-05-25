Sample code to deploy to Azure App Service using Maven and from terminal

1- Login from terminal first

Az Login

2 - Run this to let Azure create the plugin section for you in pom.xml

mvn com.microsoft.azure:azure-webapp-maven-plugin:2.11.0:config


3- Verify plugin section added with app service details, if so, run last command to deploy into it


mvn package azure-webapp:deploy
