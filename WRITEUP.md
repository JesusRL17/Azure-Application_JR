# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*

App Service
Cost is free with the plan Free (F1) for this applicaiton and it should be enough with the current size and operation of the application.
Scalability can be achieved by changing the current plan to a basic plan altough scalling has to be done manually or a Premium Plan so this can configured with Rules.
Availability, F1 free plan does not provides and SLA, but for Basic, Standar and Premiums plans the availability will be 99.95%.
Workflow is very simple using the deployment Center, and under Continuous Deployment we just have to select Git hub and login with the git hub acount, select the desired repository and branch and this will create automatically the workflow file to the repostory. Once changes are commited to the branch selected build and deploy will start immediately.

VM
Cost for the basic plan of is 3.80 per month.
Scalability has to be made with Scale Sets.
We can use Availability zones, in this case Azure offers 99.99 up time.



- *Choose the appropriate solution (VM or App Service) for deploying the app*

I choose to use an App service for my solution.
- *Justify your choice*

One reason to choose App service over VM is the size and operation of the application, at this point we dont need that much control over the OS or the Hardware, also the cost is free with the current plan so this is also benefit for the scenario. It was easier and faster to deploy the app in the app service compared with the effort to do it in the VM and Python is supported there was not problem.

I could focus more in develpment of the app rather than hardare or capabilites of the VM.


### Assess app changes that would change your decision.

Definetly I would choose VM if language was not supported by AppService and if needed more control over the Hardware.
