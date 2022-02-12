# Aka-Application
Technical details and Instructions:
* I used .NET 5.0 framework and Visual Studio 2019.

The  AkaMonitoring Solution includes 3 projects: 
1.	Monitor 
2.	Simulator 
3.	JsonConfigurationCreator

1)In order to test Aka System, Please run Monitor project first and then Simulator project second. The System supports exactly this order of run.

2) Please Run the monitor project only from Visual studio.

3) The configuration is in Json format. There are 2 Json file configurations, 
Monitor looking for configuration file at the following relative location:  
simulator\monitor\config\AcaMonitorConfiguration.json
Simulator looking for configuration file at the following relative location:
simulator\simulator\config\AcaSimulatorConfiguration.json

The configuration files are already in the solution at the right locations.
Running   JsonConfigurationCreator project is optional and it needed only in order to regenerate configuration files. 
Executing JsonConfigurationCreator creates 2 new configuration files:
AcaMonitorConfiguration.json and  AcaSimulatorConfiguration.json. 
The process creates them in the executing repository of JsonConfigurationCreator  project.

4)Currently logs location is the “logs” subfolder of the executable repository of Monitor project.

5)Scrolling of the displayed messages in UI is not implemented. 

