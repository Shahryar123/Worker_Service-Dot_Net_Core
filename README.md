# Worker Service ASP DOTNET CORE 7.0

A Worker Service is a real process, but is intended as a background service for a front-end application.

It starts with the application and stops with the application.

The Background Worker Class allows you to set a thread continuously running in the background and communicating with the main thread whenever required.

They aim to improve reliability by providing offline access, as well as boost page performance.

Creating Worker Service to create logs file using Nlog

**Steps to Implement Worker Service in DotNet Core**
	
	1. Create a worker service project in asp.net core
	2. Download Nuget package for Nlog
	3. Create a config file and define path for the logs file
	4. Create a class in which you want to create logs
	5. Execute the project
	
Note till the project is running the worker service update the logs file so for continuously running in the background we used nssm.
NSSM is a service manager that create your project into background windows service.

For NSSM we need to publish our project and copy the nssm.exe in the publish folder.

**Execute the following commands in cmd to the root folder**

	1. nssm install <Service_Name>
	2. Provide path to your exe 
	3. Service is created but not running
	4. Go to Task manager and start running your service 

Now it will working and create logs to the specified folder

#Happy Coding :+1: :+1:
