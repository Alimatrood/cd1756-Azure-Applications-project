# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice*

- Cost: Azure app service can actually be more expensive compared to VMs. An example comparision will be as the following: 

App service - P1v3 plan is a DsV2 Azure VM 2 Core, 8 GB RAM, 250GB Storage will cost $275.21 USD per month.

VMs - DsV5 Series Azure VM 2 Cores, 8 GB RAM,  256 GB Standard SSD Storage will cost $182.92 USD per month.

VMs are only charged on disk costs when stopped. However, azure app service will continue charging even though apps are not used or when stopped (do not offer pay as you go).


- Scalability: 
VMs have horizontal scaling which can be achieved by running large number of VMs, to handle load. In addition, vertical scaling can be acheived by increasing the capacity of memory, CPU speed, disk space and network.

In App Service, there is built-in autoscaling.

- Availability:
Both VMs and App Services are available can be existed in multiple regions.


VMs are Infrastructure as a Service, which will give the control over operating system, while in App Services you only have the control over the app and data.


I have chosen App Service since the app is simple, does not need big computational power, and does not need control over the operating system of it.

### Assess app changes that would change your decision.

*Detail how the app and any other needs would have to change for you to change your decision in the last section.* 

- When the app requires more computational power.
- When we need more control over the operating system.
- When the app is developed using a programming language that is not supported by the App Service.