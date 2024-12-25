### You are implementing a software as a service (SaaS) ASP.NET Core web service that will run as an Azure Web App. The web service will use an on-premises SQL Server database for storage. The web service also includes a WebJob that processes data updates. Four customers will use the web service. Each instance of the WebJob processes data for a single customer and must run as a singleton instance. Each deployment must be tested by using deployment slots prior to serving production data. Azure costs must be minimized. Azure resources must be located in an isolated network. You need to configure the App Service plan for the Web App. How should you configure the App Service plan?

![Question 1](images/question1.jpeg)

- [ ] Number of VM instances: 2. Pricing tier: Isolated.
- [ ] Number of VM instances: 8. Pricing tier: Standard.
- [ ] Number of VM instances: 16. Pricing tier: Premium.
- [x] Number of VM instances: 4. Pricing tier: Isolated.
- [ ] Number of VM instances: 4. Pricing tier: Consumption.


### You are a developer for a software as a service (SaaS) company that uses an Azure Function to process orders. The Azure Function currently runs on an Azure Function app that is triggered by an Azure Storage queue. You are preparing to migrate the Azure Function to Kubernetes using Kubernetes-based Event Driven Autoscaling (KEDA). You need to configure Kubernetes Custom Resource Definitions (CRD) for the Azure Function. Which CRDs should you configure?

![Question 2](images/question2.jpeg)

- [x] Box 1, CRD type: Deployment. Box 2, CRD type: ScaledObject. Box 3, CRD type: Secret.
- [ ] Box 1, CRD type: Secret. Box 2, CRD type: ScaledObject. Box 3, CRD type: Secret.
- [ ] Box 1, CRD type: TriggerAuthentication. Box 2, CRD type: Deployment. Box 3, CRD type: Secret.
- [ ] Box 1, CRD type: Deployment. Box 2, CRD type: ScaledObject. Box 3, CRD type: TriggerAuthentication.


### You are creating a CLI script that creates an Azure web app and related services in Azure App Service. The web app uses the following variables. You need to automatically deploy code from GitHub to the newly created web app. How should you complete the script?

![Question 3 part 1](images/question3_1.png)
![Question 3 part 2](images/question3_2.jpeg)

- [ ] Box 1: az webapp. Box 2: az webapp create. Box 3: git clone $gitrepo. Box 4: az webapp. Box 5: --plan $webappname
- [x] Box 1: az appservice plan create. Box 2: az webapp create. Box 3: --plan $webappname. Box 4: az webapp deployment. Box 5: --repo-url $gitrepo --branch master --manual-integration
- [ ] Box 1: az appservice plan create. Box 2: az webapp deployment. Box 3: --plan $webappname. Box 4: az webapp deployment. Box 5: --repo-url $gitrepo --branch master --manual-integration
- [ ] Box 1: az group delete. Box 2: az webapp create. Box 3: git clone $gitrepo. Box 4: az appservice plan create. Box 5: git clone $gitrepo


### You develop a software as a service (SaaS) offering to manage photographs. Users upload photos to a web service which then stores the photos in Azure Storage Blob storage. The storage account type is General-purpose V2. When photos are uploaded, they must be processed to produce and save a mobile-friendly version of the image. The process to produce a mobile-friendly version of the image must start in less than one minute. You need to design the process that starts the photo processing. Solution: Trigger the photo processing from Blob storage events. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop and deploy an Azure App Service API app to a Windows-hosted deployment slot named Development. You create additional deployment slots named Testing and Production. You enable auto swap on the Production deployment slot. You need to ensure that scripts run and resources are available before a swap operation occurs. Solution: Update the web.config file to include the applicationInitialization configuration element. Specify custom initialization actions to run the scripts. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You develop and deploy an Azure App Service API app to a Windows-hosted deployment slot named Development. You create additional deployment slots named Testing and Production. You enable auto swap on the Production deployment slot. You need to ensure that scripts run and resources are available before a swap operation occurs. Solution: Enable auto swap for the Testing slot. Deploy the app to the Testing slot. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop and deploy an Azure App Service API app to a Windows-hosted deployment slot named Development. You create additional deployment slots named Testing and Production. You enable auto swap on the Production deployment slot. You need to ensure that scripts run and resources are available before a swap operation occurs. Solution: Disable auto swap. Update the app with a method named statuscheck to run the scripts. Re-enable auto swap and deploy the app to the Production slot. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You develop a software as a service (SaaS) offering to manage photographs. Users upload photos to a web service which then stores the photos in Azure Storage Blob storage. The storage account type is General-purpose V2. When photos are uploaded, they must be processed to produce and save a mobile-friendly version of the image. The process to produce a mobile-friendly version of the image must start in less than one minute. You need to design the process that starts the photo processing. Solution: Convert the Azure Storage account to a BlockBlobStorage storage account. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing an Azure Web App. You configure TLS mutual authentication for the web app. You need to validate the client certificate in the web app.

![Question 9](images/question9.jpeg)

- [ ] Client certificate location: Client cookie. Encoding type: URL.
- [ ] Client certificate location: HTTP message body. Encoding type: Base64.
- [ ] Client certificate location: HTTP request header. Encoding type: Unicode.
- [x] Client certificate location: HTTP request header. Encoding type: Base64.


### You are developing a Docker/Go using Azure App Service Web App for Containers. You plan to run the container in an App Service on Linux. You identify a Docker container image to use. None of your current resource groups reside in a location that supports Linux. You must minimize the number of resource groups required. You need to create the application and perform an initial deployment. Which three Azure CLI commands should you use to develop the solution?

![Question 10](images/question10.png)

- [ ] Box 1: az webapp create. Box 2: az appservice plan create. Box 3: az group create.
- [ ] Box 1: az appservice plan create. Box 2: az group create. Box 3: az group update.
- [x] Box 1: az group create. Box 2: az appservice plan create. Box 3: az webapp create.
- [ ] Box 1: az appservice plan create. Box 2: az webapp create. Box 3: az webapp update.


### Fourth Coffee has an ASP.NET Core web app that runs in Docker. The app is mapped to the www.fourthcoffee.com domain. Fourth Coffee is migrating this application to Azure. You need to provision an App Service Web App to host this docker image and map the custom domain to the App Service web app. A resource group named FourthCoffeePublicWebResourceGroup has been created in the WestUS region that contains an App Service Plan named AppServiceLinuxDockerPlan. Which order should the CLI commands be used to develop the solution?

![Question 11](images/question11.jpeg)

- [x] Box 1: #/bin/bash appName='FourthCoffeePublicWeb$random' location='WestUS' dockerHubContainerPath='FourthCoffee/publicweb:v1' fqdn='http://www.fourthcoffee.com'>www.fourthcoffee.com. Box 2: az webapp create --name $appName --plan AppServiceLinuxDockerPlan --resource-group fourthCoffeePublicWebResourceGroup. Box 3: az webapp config container set --docker-custom-image-name $dockerHubContainerPath --name $appName --resource-group fourthCoffeePublicWebResourceGroup. Box 4: az webapp config hostname add --webapp-name $appName --resource-group fourthCoffeePublicWebResourceGroup --hostname $fqdn.
- [ ] Box 1: #/bin/bash appName='FourthCoffeePublicWeb$random' location='WestUS' dockerHubContainerPath='FourthCoffee/publicweb:v1' fqdn='http://www.fourthcoffee.com'>www.fourthcoffee.com. Box 2: az webapp create --name $appName --plan AppServiceLinuxDockerPlan --resource-group fourthCoffeePublicWebResourceGroup. Box 3: az webapp config hostname add --webapp-name $appName --resource-group fourthCoffeePublicWebResourceGroup --hostname $fqdn. Box 4: az webapp config container set --docker-custom-image-name $dockerHubContainerPath --name $appName --resource-group fourthCoffeePublicWebResourceGroup.
- [ ] Box 1: az webapp config container set --docker-custom-image-name $dockerHubContainerPath --name $appName --resource-group fourthCoffeePublicWebResourceGroup. Box 2: az webapp create --name $appName --plan AppServiceLinuxDockerPlan --resource-group fourthCoffeePublicWebResourceGroup. Box 3: az webapp config hostname add --webapp-name $appName --resource-group fourthCoffeePublicWebResourceGroup --hostname $fqdn.. Box 4: #/bin/bash appName='FourthCoffeePublicWeb$random' location='WestUS' dockerHubContainerPath='FourthCoffee/publicweb:v1' fqdn='http://www.fourthcoffee.com'>www.fourthcoffee.com..
- [ ] Box 1: az webapp config hostname add --webapp-name $appName --resource-group fourthCoffeePublicWebResourceGroup --hostname $fqdn. Box 2: az webapp create --name $appName --plan AppServiceLinuxDockerPlan --resource-group fourthCoffeePublicWebResourceGroup. Box 3: #/bin/bash appName='FourthCoffeePublicWeb$random' location='WestUS' dockerHubContainerPath='FourthCoffee/publicweb:v1' fqdn='http://www.fourthcoffee.com'>www.fourthcoffee.com. Box 4: az webapp config container set --docker-custom-image-name $dockerHubContainerPath --name $appName --resource-group fourthCoffeePublicWebResourceGroup.


### You are developing a serverless Java application on Azure. You create a new Azure Key Vault to work with secrets from a new Azure Functions application. The application must meet the following requirements: Reference the Azure Key Vault without requiring any changes to the Java code. Dynamically add and remove instances of the Azure Functions host based on the number of incoming application events. Ensure that instances are perpetually warm to avoid any cold starts. Connect to a VNet. Authentication to the Azure Key Vault instance must be removed if the Azure Function application is deleted. You need to grant the Azure Functions application access to the Azure Key Vault. Which three actions should you perform in sequence?

![Question 12](images/question12.png)

- [ ] Box 1: Create the Azure Functions app with a Consumption plan type. Box 2: Create an access policy in Azure Key Vault for the application identity. Box 3: Create a user-assigned managed identity for the application.
- [x] Box 1: Create the Azure Functions app with a Premium plan type. Box 2: Create a system-assigned managed identity for the application. Box 3: Create an access policy in Azure Key Vault for the application identity.
- [ ] Box 1: Create the Azure Functions app with a Consumption plan type. Box 2: Create a user-assigned managed identity for the application. Box 3: Create an access policy in Azure Key Vault for the application identity.
- [ ] Box 1: Create the Azure Functions app with a Premium plan type. Box 2: Create a user-assigned managed identity for the application. Box 3: Create an access policy in Azure Key Vault for the application identity.


### You develop a website. You plan to host the website in Azure. You expect the website to experience high traffic volumes after it is published. You must ensure that the website remains available and responsive while minimizing cost. You need to deploy the website. What should you do?

- [ ] Deploy the website to a virtual machine. Configure the virtual machine to automatically scale when the CPU load is high.
- [ ] Deploy the website to an App Service that uses the Shared service tier. Configure the App Service plan to automatically scale when the CPU load is high.
- [ ] Deploy the website to a virtual machine. Configure a Scale Set to increase the virtual machine instance count when the CPU load is high.
- [x] Deploy the website to an App Service that uses the Standard service tier. Configure the App Service plan to automatically scale when the CPU load is high.


### A company is developing a Java web app. The web app code is hosted in a GitHub repository located at https://github.com/Contoso/webapp. The web app must be evaluated before it is moved to production. You must deploy the initial code release to a deployment slot named staging. You need to create the web app and deploy the code. How should you complete the commands?

![Question 14](images/question14.png)

- [x] Box 1: group. Box 2: appservice plan. Box 3: webapp. Box 4: webapp deployment slot. Box 5: webapp deployment source.
- [ ] Box 1: appservice plan. Box 2: group. Box 3: webapp. Box 4: webapp deployment slot. Box 5: webapp deployment source.
- [ ] Box 1: webapp. Box 2: group. Box 3: webapp deployment source. Box 4: webapp deployment slot. Box 5: appservice plan.
- [ ] Box 1: webapp. Box 2: group. Box 3: webapp deployment source. Box 4: webapp deployment slot. Box 5: appservice plan.


### You have a web service that is used to pay for food deliveries. The web service uses Azure Cosmos DB as the data store. You plan to add a new feature that allows users to set a tip amount. The new feature requires that a property named tip on the document in Cosmos DB must be present and contain a numeric value. There are many existing websites and mobile apps that use the web service that will not be updated to set the tip property for some time. How should you complete the trigger?

![Question 15](images/question15.jpeg)

- [ ] Box 1: __value();. Box 2: if (request.getValue('tip') === null) {. Box 3: __.upsertDocument(i);.
- [ ] Box 1: __readDocument()('item');. Box 2: if (!('tip' in i)) {. Box 3: __.replaceDocument(i);.
- [x] Box 1: getContext().getRequest();. Box 2: if (!('tip' in i)) {. Box 3: r.setBody(i);.
- [ ] Box 1: getContext().getRequest();. Box 2: if (isNaN(i)['tip'] || i['tip'] === null) {. Box 3: r.setValue(i);.


### You develop an HTTP triggered Azure Function app to process Azure Storage blob data. The app is triggered using an output binding on the blob. The app continues to time out after four minutes. The app must process the blob data. You need to ensure the app does not time out and processes the blob data. Solution: Use the Durable Function async pattern to process the blob data. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You develop an HTTP triggered Azure Function app to process Azure Storage blob data. The app is triggered using an output binding on the blob. The app continues to time out after four minutes. The app must process the blob data. You need to ensure the app does not time out and processes the blob data. Solution: Pass the HTTP trigger payload into an Azure Service Bus queue to be processed by a queue trigger function and return an immediate HTTP success response. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop an HTTP triggered Azure Function app to process Azure Storage blob data. The app is triggered using an output binding on the blob. The app continues to time out after four minutes. The app must process the blob data. You need to ensure the app does not time out and processes the blob data. Solution: Configure the app to use an App Service hosting plan and enable the Always On setting. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You develop a software as a service (SaaS) offering to manage photographs. Users upload photos to a web service which then stores the photos in Azure Storage Blob storage. The storage account type is General-purpose V2. When photos are uploaded, they must be processed to produce and save a mobile-friendly version of the image. The process to produce a mobile-friendly version of the image must start in less than one minute. You need to design the process that starts the photo processing. Solution: Move photo processing to an Azure Function triggered from the blob upload. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing an application that uses Azure Blob storage. The application must read the transaction logs of all the changes that occur to the blobs and the blob metadata in the storage account for auditing purposes. The changes must be in the order in which they occurred, include only create, update, delete, and copy operations and be retained for compliance reasons. You need to process the transaction logs asynchronously. What should you do?

- [ ] Process all Azure Blob storage events by using Azure Event Grid with a subscriber Azure Function app.
- [x] Enable the change feed on the storage account and process all changes for available events.
- [ ] Process all Azure Storage Analytics logs for successful blob events.
- [ ] Use the Azure Monitor HTTP Data Collector API and scan the request body for successful blob events.


### You plan to create a Docker image that runs an ASP.NET Core application named ContosoApp. You have a setup script named setupScript.ps1 and a series of application files including ContosoApp.dll. You need to create a Dockerfile document that meets the following requirements: Call setupScripts.ps1 when the container is built. Run ContosoApp.dll when the container starts. The Dockerfile document must be created in the same folder where ContosoApp.dll and setupScript.ps1 are stored. Which five commands should you use to develop the solution?

![Question 21](images/question21.png)

- [ ] Box 1: CMD ['dotnet', 'ContosoApp.dll']. Box 2: FROM microsoft/aspnetcore:latest. Box 3: RUN powershell ./setupScript.ps1. Box 4: WORKDIR /apps/ContosoApp. Box 5: COPY ./ ..
- [ ] Box 1: COPY ./ ... Box 2: RUN powershell ./setupScript.ps1. Box 3: FROM microsoft/aspnetcore:latest. Box 4: CMD ['dotnet', 'ContosoApp.dll']. Box 5: WORKDIR /apps/ContosoApp.
- [ ] Box 1: RUN powershell ./setupScript.ps1. Box 2: CMD ['dotnet', 'ContosoApp.dll']. Box 3: FROM microsoft/aspnetcore:latest. Box 4: WORKDIR /apps/ContosoApp. Box 5: COPY ./ ..
- [x] Box 1: FROM microsoft/aspnetcore:latest. Box 2: WORKDIR /apps/ContosoApp. Box 3: COPY ./ .. Box 4: RUN powershell ./setupScript.ps1. Box 5: CMD ['dotnet', 'ContosoApp.dll'].


### You are developing an Azure Function App that processes images that are uploaded to an Azure Blob container. Images must be processed as quickly as possible after they are uploaded, and the solution must minimize latency. You create code to process images when the Function App is triggered. You need to configure the Function App. What should you do?

- [ ] Use an App Service plan. Configure the Function App to use an Azure Blob Storage input trigger.
- [ ] Use a Consumption plan. Configure the Function App to use an Azure Blob Storage trigger.
- [ ] Use a Consumption plan. Configure the Function App to use a Timer trigger.
- [x] Use an App Service plan. Configure the Function App to use an Azure Blob Storage trigger.
- [ ] Use a Consumption plan. Configure the Function App to use an Azure Blob Storage input trigger.


### You are configuring a new development environment for a Java application. The environment requires a Virtual Machine Scale Set (VMSS), several storage accounts, and networking components. The VMSS must not be created until the storage accounts have been successfully created and an associated load balancer and virtual network is configured. How should you complete the Azure Resource Manager template?

![Question 23](images/question23.png)

- [x] Box 1: copyIndex. Box 2: copy. Box 3: dependsOn.
- [ ] Box 1: copy. Box 2: copyIndex. Box 3: dependsOn.
- [ ] Box 1: priority. Box 2: dependsOn. Box 3: copyIndex.
- [ ] Box 1: priority. Box 2: copyIndex. Box 3: dependsOn.


### You are developing an Azure Function App by using Visual Studio. The app will process orders input by an Azure Web App. The web app places the order information into Azure Queue Storage. You need to review the Azure Function App code shown below. Question 1: The code will log the time that the order was processed from the queue.

![Question 24](images/question24_25_26_27.png)

- [ ] Yes.
- [x] No.


### You are developing an Azure Function App by using Visual Studio. The app will process orders input by an Azure Web App. The web app places the order information into Azure Queue Storage. You need to review the Azure Function App code shown below. Question 2: When the ProcessOrders function fails, the function will retry up to five times for a given order, including the first try.

![Question 25](images/question24_25_26_27.png)

- [x] Yes.
- [ ] No.


### You are developing an Azure Function App by using Visual Studio. The app will process orders input by an Azure Web App. The web app places the order information into Azure Queue Storage. You need to review the Azure Function App code shown below. Question 3: When there are multiple orders in the queue, a batch of orders will be received from the queue and the ProcessOrders function will run multiple instances concurrently to process the orders.

![Question 26](images/question24_25_26_27.png)

- [x] Yes.
- [ ] No.


### You are developing an Azure Function App by using Visual Studio. The app will process orders input by an Azure Web App. The web app places the order information into Azure Queue Storage. You need to review the Azure Function App code shown below. Question 4: The ProcessOrders function will output the order to an Orders table in Azure Table Storage.

![Question 27](images/question24_25_26_27.png)

- [x] Yes.
- [ ] No.


### You are developing a solution for a hospital to support the following use cases: The most recent patient status details must be retrieved even if multiple users in different locations have updated the patient record. Patient health monitoring data retrieved must be the current version or the prior version. After a patient is discharged and all charges have been assessed, the patient billing record contains the final charges. You provision a Cosmos DB NoSQL database and set the default consistency level for the database account to Strong. You set the value for Indexing Mode to Consistent. You need to minimize latency and any impact to the availability of the solution. You must override the default consistency level at the query level to meet the required consistency guarantees for the scenarios. Which consistency levels should you implement?

![Question 28](images/question28.png)

- [ ] Box 1: Strong. Box 2: Consistent Prefix. Box 3: Eventual.
- [ ] Box 1: Eventual. Box 2: Strong. Box 3: Bounded Staleness.
- [ ] Box 1: Consistent Prefix. Box 2: Bounded Staleness. Box 3: Eventual.
- [x] Box 1: Strong. Box 2: Bounded Staleness. Box 3: Eventual.


### You are configuring a development environment for your team. You deploy the latest Visual Studio image from the Azure Marketplace to your Azure subscription. The development environment requires several software development kits (SDKs) and third-party components to support application development across the organization. You install and customize the deployed virtual machine (VM) for your development team. The customized VM must be saved to allow provisioning of a new team member development environment. You need to save the customized VM for future provisioning. Which tools or services should you use?

![Question 29](images/question29.png)

- [ ] Generalize the VM: Visual Studio command prompt. Store images: Azure Data Lake Storage.
- [x] Generalize the VM: Azure PowerShell. Store images: Azure Blob Storage.
- [ ] Generalize the VM: Visual Studio command prompt. Store images: Azure File Storage.
- [ ] Generalize the VM: Azure PowerShell. Store images: Azure File Storage.


### You are preparing to deploy a website to an Azure Web App from a GitHub repository. The website includes static content generated by a script. You plan to use the Azure Web App continuous deployment feature. You need to run the static generation script before the website starts serving traffic. What are two possible ways to achieve this goal?

- [ ] Add the path to the static content generation tool to WEBSITE_RUN_FROM_PACKAGE setting in the host.json file.
- [x] Add a PreBuild target in the websites csproj project file that runs the static content generation script.
- [ ] Create a file named run.cmd in the folder /run that calls a script which generates the static content and deploys the website.
- [x] Create a file named .deployment in the root of the repository that calls a script which generates the static content and deploys the website.


### You are developing an application to use Azure Blob storage. You have configured Azure Blob storage to include change feeds. A copy of your storage account must be created in another region. Data must be copied from the current storage account to the new storage account directly between the storage servers. You need to create a copy of the storage account in another region and copy the data. In which order should you perform the actions?

![Question 31](images/question31.jpeg)

- [ ] Box 1: Create a new template deployment. Box 2: Export a Resource Manager template. Box 3: Modify the template by changing the storage account name and region. Box 4: Deploy the template to create a new storage account in the target region. Box 5: Use AZCopy to copy the data to the new storage account.
- [ ] Box 1: Use AZCopy to copy the data to the new storage account. Box 2: Create a new template deployment. Box 3: Modify the template by changing the storage account name and region. Box 4: Deploy the template to create a new storage account in the target region. Box 5: Export a Resource Manager template.
- [x] Box 1: Export a Resource Manager template. Box 2: Create a new template deployment. Box 3: Modify the template by changing the storage account name and region. Box 4: Deploy the template to create a new storage account in the target region. Box 5: Use AZCopy to copy the data to the new storage account.
- [ ] Box 1: Use AZCopy to copy the data to the new storage account. Box 2: Create a new template deployment. Box 3: Modify the template by changing the storage account name and region. Box 4: Deploy the template to create a new storage account in the target region. Box 5: Export a Resource Manager template.


### You are preparing to deploy an Azure virtual machine (VM)-based application. The VMs that run the application have the following requirements: When a VM is provisioned the firewall must be automatically configured before it can access Azure resources. Supporting services must be installed by using an Azure PowerShell script that is stored in Azure Storage. You need to ensure that the requirements are met. Which features should you use?

![Question 32](images/question32.jpeg)

- [ ] Firewall configuration: Run Command. Supporting services script: Hybrid Runbook Worker.
- [ ] Firewall configuration: Customer Script Extension. Supporting services script: Serial console.
- [x] Firewall configuration: Run Command. Supporting services script: Customer Script Extension.
- [ ] Firewall configuration: Hybrid Runbook Worker. Supporting services script: Customer Script Extension.


### A company is developing a Node.js web app. The web app code is hosted in a GitHub repository located at https://github.com/TailSpinToys/webapp. The web app must be reviewed before it is moved to production. You must deploy the initial code release to a deployment slot named review. You need to create the web app and deploy the code. How should you complete the commands?

![Question 33](images/question33.jpeg)

- [ ] Box 1: New-AzWebAppSlot. Box 2: New-AzWebApp. Box 3: New-AzAppServicePlan. Box 4: New-AzResourceGroup.
- [x] Box 1: New-AzResourceGroup. Box 2: New-AzAppServicePlan. Box 3: New-AzWebApp. Box 4: New-AzWebAppSlot.
- [ ] Box 1: New-AzWebAppSlot. Box 2: New-AzAppServicePlan. Box 3: New-AzWebApp. Box 4: New-AzResourceGroup.
- [ ] Box 1: New-AzResourceGroup. Box 2: New-AzAppServicePlan. Box 3: New-AzWebAppSlot. Box 4: New-AzWebApp.


### You are developing an application that needs access to an Azure virtual machine (VM). The access lifecycle for the application must be associated with the VM service instance. You need to enable managed identity for the VM. How should you complete the PowerShell segment?

![Question 34](images/question34.jpeg)

- [ ] Box 1: -AssignIdentity:. Box 2: $SystemAssigned.
- [ ] Box 1: -AssignIdentity:. Box 2: $UserAssigned.
- [x] Box 1: -IdentityId: (note: screenshot has mistake, it should be '-IdentityType:' in the dropdown). Box 2: $SystemAssigned.
- [ ] Box 1: -IdentityId: (note: screenshot has mistake, it should be '-IdentityType:' in the dropdown). Box 2: $UserAssigned.


### You develop a software as a service (SaaS) offering to manage photographs. Users upload photos to a web service which then stores the photos in Azure Storage Blob storage. The storage account type is General-purpose V2. When photos are uploaded, they must be processed to produce and save a mobile-friendly version of the image. The process to produce a mobile-friendly version of the image must start in less than one minute. You need to design the process that starts the photo processing. Solution: Create an Azure Function app that uses the Consumption hosting model and that is triggered from the blob upload. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop and deploy an Azure App Service API app to a Windows-hosted deployment slot named Development. You create additional deployment slots named Testing and Production. You enable auto swap on the Production deployment slot. You need to ensure that scripts run and resources are available before a swap operation occurs. Solution: Update the app with a method named statuscheck to run the scripts. Update the app settings for the app. Set the WEBSITE_SWAP_WARMUP_PING_PATH and WEBSITE_SWAP_WARMUP_PING_STATUSES with a path to the new method and appropriate response codes. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You create the following PowerShell script. Question 1: A log alert is created that sends an email when the CPU percentage is above 60 percent for five minutes.

![Question 37](images/question37_38_39.png)

- [ ] Yes.
- [x] No.


### You create the following PowerShell script. Question 2: A log alert is created that sends an email when the number of machine heartbeats in the past hour is less than five.

![Question 38](images/question37_38_39.png)

- [x] Yes.
- [ ] No.


### You create the following PowerShell script. Question 3: The log alert is scheduled to run every two hours.

![Question 39](images/question37_38_39.png)

- [ ] Yes.
- [x] No.


### You are developing an Azure Function app. The app must meet the following requirements: Enable developers to write the functions by using the Rust language. Declaratively connect to an Azure Blob Storage account. You need to implement the app. Which Azure Function app features should you use?

![Question 40](images/question40.png)

- [ ] Enable developers to write the functions by using the Rust language: Hosting plan. Declaratively connect to an Azure Blog Storage account: Custom handler.
- [ ] Enable developers to write the functions by using the Rust language: Runtime. Declaratively connect to an Azure Blog Storage account: Policy.
- [ ] Enable developers to write the functions by using the Rust language: Custom handler. Declaratively connect to an Azure Blog Storage account: Trigger.
- [x] Enable developers to write the functions by using the Rust language: Custom handler. Declaratively connect to an Azure Blog Storage account: Extension bundle.


### You are developing an ASP.NET Core web application. You plan to deploy the application to Azure Web App for Containers. The application needs to store runtime diagnostic data that must be persisted across application restarts. You have the following code. You need to configure the application settings so that diagnostic data is stored as required. How should you configure the web app's settings?

![Question 41 part 1](images/question41_1.jpeg)
![Question 41 part 2](images/question41_2.jpeg)

- [x] App setting: WEBSITES_ENABLE_APP_SERVICE_STORAGE. Value: /home.
- [ ] App setting: WEBSITES_ENABLE_APP_SERVICE_STORAGE. Value: /local.
- [ ] App setting: LOCALAPPDATA. Value: D:\home.
- [ ] App setting: DOTNET_HOSTING_OPTIMIZATION_CACHE. Value: D:\home.


### You are developing a web app that is protected by Azure Web Application Firewall (WAF). All traffic to the web app is routed through an Azure Application Gateway instance that is used by multiple web apps. The web app address is contoso.azurewebsites.net. All traffic must be secured with SSL. The Azure Application Gateway instance is used by multiple web apps. You need to configure the Azure Application Gateway for the web app. Which two actions should you perform?

- [x] In the Azure Application Gateway's HTTP setting, enable the Use for App service setting.
- [ ] Convert the web app to run in an Azure App service environment (ASE).
- [ ] Add an authentication certificate for contoso.azurewebsites.net to the Azure Application Gateway.
- [x] In the Azure Application Gateway's HTTP setting, set the value of the Override backend path option to contoso22.azurewebsites.net.


### You develop a software as a service (SaaS) offering to manage photographs. Users upload photos to a web service which then stores the photos in Azure Storage Blob storage. The storage account type is General-purpose V2. When photos are uploaded, they must be processed to produce and save a mobile-friendly version of the image. The process to produce a mobile-friendly version of the image must start in less than one minute. You need to design the process that starts the photo processing. Solution: Use the Azure Blob Storage change feed to trigger photo processing. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### A company develops a series of mobile games. All games use a single leaderboard service. You have the following requirements: Code must be scalable and allow for growth. Each record must consist of a playerId, gameId, score, and time played. When users reach a new high score, the system will save the new score using the SaveScore function below. Each game is assigned an Id based on the series title. You plan to store customer information in Azure Cosmos DB. The following data already exists in the database: You develop the following code to save scores in the data store. (Line numbers are included for reference only.) You develop the following code to query the database. (Line numbers are included for reference only.). Question 1: SaveScore will work with Cosmos DB.

![Question 44 part 1](images/question44_45_46_47_1.png)
![Question 44 part 2](images/question44_45_46_47_2.png)
![Question 44 part 3](images/question44_45_46_47_3.jpeg)

- [x] Yes.
- [ ] No.


### A company develops a series of mobile games. All games use a single leaderboard service. You have the following requirements: Code must be scalable and allow for growth. Each record must consist of a playerId, gameId, score, and time played. When users reach a new high score, the system will save the new score using the SaveScore function below. Each game is assigned an Id based on the series title. You plan to store customer information in Azure Cosmos DB. The following data already exists in the database: You develop the following code to save scores in the data store. (Line numbers are included for reference only.) You develop the following code to query the database. (Line numbers are included for reference only.). Question 2: SaveScore will update and replace a record if one already exists with the same playerId and gameId.

![Question 45 part 1](images/question44_45_46_47_1.png)
![Question 45 part 2](images/question44_45_46_47_2.png)
![Question 45 part 3](images/question44_45_46_47_3.jpeg)

- [ ] Yes.
- [x] No.


### A company develops a series of mobile games. All games use a single leaderboard service. You have the following requirements: Code must be scalable and allow for growth. Each record must consist of a playerId, gameId, score, and time played. When users reach a new high score, the system will save the new score using the SaveScore function below. Each game is assigned an Id based on the series title. You plan to store customer information in Azure Cosmos DB. The following data already exists in the database: You develop the following code to save scores in the data store. (Line numbers are included for reference only.) You develop the following code to query the database. (Line numbers are included for reference only.). Question 3: Leader board data for the game will be automatically partitioned using gameId.

![Question 46 part 1](images/question44_45_46_47_1.png)
![Question 46 part 2](images/question44_45_46_47_2.png)
![Question 46 part 3](images/question44_45_46_47_3.jpeg)

- [ ] Yes.
- [x] No.


### A company develops a series of mobile games. All games use a single leaderboard service. You have the following requirements: Code must be scalable and allow for growth. Each record must consist of a playerId, gameId, score, and time played. When users reach a new high score, the system will save the new score using the SaveScore function below. Each game is assigned an Id based on the series title. You plan to store customer information in Azure Cosmos DB. The following data already exists in the database: You develop the following code to save scores in the data store. (Line numbers are included for reference only.) You develop the following code to query the database. (Line numbers are included for reference only.). Question 4: SaveScore will store the values for the gameId and playerId parameters in the database.

![Question 47 part 1](images/question44_45_46_47_1.png)
![Question 47 part 2](images/question44_45_46_47_2.png)
![Question 47 part 3](images/question44_45_46_47_3.jpeg)

- [x] Yes.
- [ ] No.


### You are developing a solution that uses the Azure Storage Client library for .NET. You have the following code: (Line numbers are included for reference only.). Question 1: The code creates an infinite lease.

![Question 48](images/question48_49_50.jpeg)

- [x] Yes.
- [ ] No.


### You are developing a solution that uses the Azure Storage Client library for .NET. You have the following code: (Line numbers are included for reference only.). Question 2: The code at line 06 always creates a new blob.

![Question 49](images/question48_49_50.jpeg)

- [ ] Yes.
- [x] No.


### You are developing a solution that uses the Azure Storage Client library for .NET. You have the following code: (Line numbers are included for reference only.). Question 3: The finally block releases the lease.

![Question 50](images/question48_49_50.jpeg)

- [x] Yes.
- [ ] No.


### You are building a website that uses Azure Blob storage for data storage. You configure Azure Blob storage lifecycle to move all blobs to the archive tier after 30 days. Customers have requested a service-level agreement (SLA) for viewing data older than 30 days. You need to document the minimum SLA for data recovery. Which SLA should you use?

- [ ] At least two days.
- [x] Between one and 15 hours.
- [ ] At least one day.
- [ ] Between zero and 60 minutes.


### You are developing a ticket reservation system for an airline. The storage solution for the application must meet the following requirements: Ensure at least 99.99% availability and provide low latency. Accept reservations even when localized network outages or other unforeseen failures occur. Process reservations in the exact sequence as reservations are submitted to minimize overbooking or selling the same seat to multiple travelers. Allow simultaneous and out-of-order reservations with a maximum five-second tolerance window. You provision a resource group named airlineResourceGroup in the Azure South-Central US region. You need to provision a SQL API Cosmos DB account to support the app. How should you complete the Azure CLI commands?

![Question 52](images/question52.jpeg)

- [x] Box 1: BoundedStaleness. Box 2: --enable-automatic-failover true \. Box 3: --locations 'southcentralplus=0 eastus=1 westus=2'.
- [ ] Box 1: Strong. Box 2: --enable-automatic-failover true \. Box 3: --locations 'southcentralplus=0 eastus=1 westus=2'.
- [ ] Box 1: BoundedStaleness. Box 2: --enable-automatic-failover true \. Box 3: --locations 'southcentralus'.
- [ ] Box 1: Strong. Box 2: --kind 'MongoDB' \. Box 3: --locations 'southcentralus'.


### You are preparing to deploy a Python website to an Azure Web App using a container. The solution will use multiple containers in the same container group. The Dockerfile that builds the container is as follows. You build a container by using the following command. The Azure Container Registry instance named images is a private registry. The user name and password for the registry is admin. The Web App must always run the same version of the website regardless of future builds. You need to create an Azure Web App to run the website. How should you complete the commands?

![Question 53 part 1](images/question53_1.png)
![Question 53 part 2](images/question53_2.png)
![Question 53 part 3](images/question53_3.jpeg)

- [ ] Box 1: --sku B1 --hyper-v. Box 2: --deployment-source-url images.azurecr.io/website:1.0.0. Box 3: container set --docker-registry-server-url https://images.azurecr.io -u admin -p admin.
- [x] Box 1: --sku B1 --is-linux. Box 2: --deployment-container-image-name images.azurecr.io/website:v1.0.0. Box 3: container set --docker-registry-server-url https://images.azurecr.io -u admin -p admin.
- [ ] Box 1: --tags container. Box 2: --deployment-source-url images.azurecr.io/website:latest. Box 3: set --python-version 2.7 --generic-configurations user=admin password=admin.
- [ ] Box 1: --sku SHARED. Box 2: --deployment-container-image-name images.azurecr.io/website:latest. Box 3: set --python-version 3.6 --generic-configurations user=admin password=admin.


### You are developing a back-end Azure App Service that scales based on the number of messages contained in a Service Bus queue. A rule already exists to scale up the App Service when the average queue length of unprocessed and valid queue messages is greater than 1000. You need to add a new rule that will continuously scale down the App Service as long as the scale up condition is not met. How should you configure the Scale rule?

![Question 54](images/question54.jpeg)

- [x] Metric source: Service Bus queue. Metric name: Active Message Count. Time train statistic: Average. Operator: Less than or equal to. Operation: Decrease count by.
- [ ] Metric source: Service Bus queue. Metric name: Active Message Count. Time train statistic: Count. Operator: Less than or equal to. Operation: Decrease count by.
- [ ] Metric source: Storage queue. Metric name: Active Message Count. Time train statistic: Count. Operator: Less than. Operation: Decrease count to.
- [ ] Metric source: Service Bus queue. Metric name: Message Count. Time train statistic: Average. Operator: Greater than. Operation: Decrease count to.


### You have an application that uses Azure Blob storage. You need to update the metadata of the blobs. Which three methods should you use to develop the solution?

![Question 55](images/question55.jpeg)

- [ ] Box 1: Metadata.Add. Box 2: SetMetadataAsync. Box 3: SetPropertiesAsync.
- [ ] Box 1: Metadata.Add. Box 2: SetMetadataAsync. Box 3: UploadFileStream.
- [ ] Box 1: Metadata.Add. Box 2: FetchAttributesAsync. Box 3: SetPropertiesAsync.
- [x] Box 1: FetchAttributesAsync. Box 2: Metadata.Add. Box 3: SetMetadataAsync.


### You are developing an Azure solution to collect point-of-sale (POS) device data from 2,000 stores located throughout the world. A single device can produce 2 megabytes (MB) of data every 24 hours. Each store location has one to five devices that send data. You must store the device data in Azure Blob storage. Device data must be correlated based on a device identifier. Additional stores are expected to open in the future. You need to implement a solution to receive the device data. Solution: Provision an Azure Event Grid. Configure the machine identifier as the partition key and enable capture. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop Azure solutions. A .NET application needs to receive a message each time an Azure virtual machine finishes processing data. The messages must NOT persist after being processed by the receiving application. You need to implement the .NET object that will receive the messages. Which object should you use?

- [x] QueueClient.
- [ ] SubscriptionClient.
- [ ] TopicClient.
- [ ] CloudQueueClient.


### You are maintaining an existing application that uses an Azure Blob GPv1 Premium storage account. Data older than three months is rarely used. Data newer than three months must be available immediately. Data older than a year must be saved but does not need to be available immediately. You need to configure the account to support a lifecycle management rule that moves blob data to archive storage for data not modified in the last year. Which three actions should you perform in sequence?

![Question 58](images/question58.jpeg)

- [ ] Box 1: Upgrade the storage account to GPv2. Box 2: Copy the data to be archived to a Standard GPv2 storage account and then delete the data from the original storage account. Box 3: Change the storage account access tier from hot to cool.
- [x] Box 1: Upgrade the storage account to GPv2. Box 2: Create a new GPv2 Standard account and set its default access tier level to cool. Box 3: Copy the data to be archived to a Standard GPv2 storage account and then delete the data from the original storage account.
- [ ] Box 1: Upgrade the storage account to GPv2. Box 2: Copy the data to be archived to a Standard GPv2 storage account and then delete the data from the original storage account. Box 3: Create a new GPv2 Standard account and set its default access tier level to cool.
- [ ] Box 1: Create a new GPv2 Standard account and set its default access tier level to cool. Box 2: Copy the data to be archived to a Standard GPv2 storage account and then delete the data from the original storage account. Box 3: Upgrade the storage account to GPv2.


### You develop Azure solutions. You must connect to a No-SQL globally-distributed database by using the .NET API. You need to create an object to configure and execute requests in the database. Which code segment should you use?

- [ ] new Container(EndpointUri, PrimaryKey);.
- [ ] new Database(EndpointUri, PrimaryKey);.
- [x] new CosmosClient(EndpointUri, PrimaryKey);.


### You have an existing Azure storage account that stores large volumes of data across multiple containers. You need to copy all data from the existing storage account to a new storage account. The copy process must meet the following requirements: Automate data movement. Minimize user input required to perform the operation. Ensure that the data movement process is recoverable. What should you use?

- [x] AzCopy.
- [ ] Azure Storage Explorer.
- [ ] Azure portal.
- [ ] .NET Storage Client Library.


### You are developing a web service that will run on Azure virtual machines that use Azure Storage. You configure all virtual machines to use managed identities. You have the following requirements: Secret-based authentication mechanisms are not permitted for accessing an Azure Storage account. Must use only Azure Instance Metadata Service endpoints. You need to write code to retrieve an access token to access Azure Storage.

![Question 61](images/question61.jpg)

- [ ] Code segment 1: <http://localhost::50342/oauth2/token>. Code segment 2: new MultipartContent(payload);.
- [ ] Code segment 1: <http://localhost/metadata/identity/oauth2/token>. Code segment 2: JsonConvert.DeserializeObject<Dictionary<string, string>>(payload);.
- [ ] Code segment 1: <http://169.254.169.254:50432/metadata/identity/oauth2/token>. Code segment 2: new NetworkCredential('Azure', payload);.
- [x] Code segment 1: <http://169.254.169.254:50432/metadata/identity/oauth2/token>. Code segment 2: JsonConvert.DeserializeObject<Dictionary<string, string>>(payload);.


### You are developing a new page for a website that uses Azure Cosmos DB for data storage. The feature uses documents that have the following format. You must display data for the new page in a specific order. You create the following query for the page. You need to configure a Cosmos DB policy to support the query. How should you configure the policy?

![Question 62 part 1](images/question62_1.png)
![Question 62 part 2](images/question62_2.png)
![Question 62 part 2](images/question62_3.png)

- [ ] Box 1: orderBy. Box 2: compositeIndexes.
- [x] Box 1: compositeIndexes. Box 2: descending.
- [ ] Box 1: compositeIndexes. Box 2: ascending.
- [ ] Box 1: ascending. Box 2: descending.


### You are building a traffic monitoring system that monitors traffic along six highways. The system produces time series analysis-based reports for each highway. Data from traffic sensors are stored in Azure Event Hub. Traffic data is consumed by four departments. Each department has an Azure Web App that displays the time series-based reports and contains a WebJob that processes the incoming data from Event Hub. All Web Apps run on App Service Plans with three instances. Data throughput must be maximized. Latency must be minimized. You need to implement the Azure Event Hub. Which settings should you use?

![Question 63](images/question63.png)

- [x] Number of partitions: 6. Partition Key: Highway.
- [ ] Number of partitions: 12. Partition Key: VM name.
- [ ] Number of partitions: 12. Partition Key: Highway.
- [ ] Number of partitions: 6 Partition Key: Department.


### You are developing a microservices solution. You plan to deploy the solution to a multinode Azure Kubernetes Service (AKS) cluster. You need to deploy a solution that includes the following features: reverse proxy capabilities configurable traffic routing TLS termination with a custom certificate. Which components should you use?

![Question 64](images/question64.jpg)

- [ ] Deploy solution: Draft. View cluster and external addressing: CoreDNS. Implement a single, public IP endpoint that is routed to multiple microservices: Vrtual Kubelet.
- [ ] Deploy solution: Helm. View cluster and external addressing: Brigade. Implement a single, public IP endpoint that is routed to multiple microservices: kubeCtl.
- [x] Deploy solution: Helm. View cluster and external addressing: KubeCtl. Implement a single, public IP endpoint that is routed to multiple microservices: Ingress Controller.
- [ ] Deploy solution: Ingress Controller. View cluster and external addressing: Helm. Implement a single, public IP endpoint that is routed to multiple microservices: Brigade.


### You are implementing an order processing system. A point of sale application publishes orders to topics in an Azure Service Bus queue. The Label property for the topic includes the following data. The system has the following requirements for subscriptions. You need to implement filtering and maximize throughput while evaluating filters. Which filter types should you implement?

![Question 65 part 1](images/question65_1.png)
![Question 65 part 2](images/question65_2.png)
![Question 65 part 3](images/question65_3.png)

- [x] Box 1: SQLFilter. Box 2: CorrelationFilter. Box 3: SQLFilter. Box 4: SQLFilter. Box 5: No Filter.
- [ ] Box 1: CorrelationFilter. Box 2: SQLFilter. Box 3: No Filter. Box 4: CorrelationFilter. Box 5: SQLFilter.
- [ ] Box 1: No Filter. Box 2: CorrelationFilter. Box 3: SQLFilter. Box 4: SQLFilter. Box 5: No Filter.
- [ ] Box 1: No Filter. Box 2: SQLFilter. Box 3: SQLFilter. Box 4: CorrelationFilter. Box 5: CorrelationFilter.


### Your company has several websites that use a company logo image. You use Azure Content Delivery Network (CDN) to store the static image. You need to determine the correct process of how the CDN and the Point of Presence (POP) server will distribute the image and list the items in the correct order. In which order do the actions occur?

![Question 66](images/question66.jpg)

- [ ] Box 1: If no edge servers in the POP have the image in cache, the POP requests the file from the origin server. Box 2: Subsequent requests for the file may be directed to the same POP using the CDN logo image URL. The POP edge server returns the file from cache if the TTL has not expired. Box 3: The origin server returns the logo image to an edge server in the POP. An edge server in the POP caches the logo image and returns the image to the client. Box 4: A user requests the image from the CDN URL. The DNS routes the request to the best performing POP location.
- [x] Box 1: A user requests the image from the CDN URL. The DNS routes the request to the best performing POP location. Box 2: If no edge servers in the POP have the image in cache, the POP requests the file from the origin server. Box 3: The origin server returns the logo image to an edge server in the POP. An edge server in the POP caches the logo image and returns the image to the client. Box 4: Subsequent requests for the file may be directed to the same POP using the CDN logo image URL. The POP edge server returns the file from cache if the TTL has not expired.
- [ ] Box 1: Subsequent requests for the file may be directed to the same POP using the CDN logo image URL. The POP edge server returns the file from cache if the TTL has not expired. Box 2: A user requests the image from the CDN URL. The DNS routes the request to the best performing POP location. Box 3: If no edge servers in the POP have the image in cache, the POP requests the file from the origin server. Box 4: The origin server returns the logo image to an edge server in the POP. An edge server in the POP caches the logo image and returns the image to the client.
- [ ] Box 1: The origin server returns the logo image to an edge server in the POP. An edge server in the POP caches the logo image and returns the image to the client. Box 2: A user requests the image from the CDN URL. The DNS routes the request to the best performing POP location. Box 3: Subsequent requests for the file may be directed to the same POP using the CDN logo image URL. The POP edge server returns the file from cache if the TTL has not expired. Box 4: If no edge servers in the POP have the image in cache, the POP requests the file from the origin server.


### You are developing an Azure Cosmos DB solution by using the Azure Cosmos DB SQL API. The data includes millions of documents. Each document may contain hundreds of properties. The properties of the documents do not contain distinct values for partitioning. Azure Cosmos DB must scale individual containers in the database to meet the performance needs of the application by spreading the workload evenly across all partitions over time. You need to select a partition key. Which two partition keys can you use?

- [ ] A single property value that does not appear frequently in the documents.
- [ ] A value containing the collection name.
- [ ] A single property value that appears frequently in the documents.
- [x] A concatenation of multiple property values with a random suffix appended.
- [x] A hash suffix appended to a property value.


### You are developing an Azure-hosted e-commerce web application. The application will use Azure Cosmos DB to store sales orders. You are using the latest SDK to manage the sales orders in the database. You create a new Azure Cosmos DB instance. You include a valid endpoint and valid authorization key to an appSettings.json file in the code project. You are evaluating the following application code: (Line number are included for reference only.). Question 1: A database named SalesOrders is created. The database will include two containers.

![Question 68](images/question68_69_70.png)

- [x] Yes.
- [ ] No.


### You are developing an Azure-hosted e-commerce web application. The application will use Azure Cosmos DB to store sales orders. You are using the latest SDK to manage the sales orders in the database. You create a new Azure Cosmos DB instance. You include a valid endpoint and valid authorization key to an appSettings.json file in the code project. You are evaluating the following application code: (Line number are included for reference only.). Question 2: Container1 will contain two items.

![Question 69](images/question68_69_70.png)

- [x] Yes.
- [ ] No.


### You are developing an Azure-hosted e-commerce web application. The application will use Azure Cosmos DB to store sales orders. You are using the latest SDK to manage the sales orders in the database. You create a new Azure Cosmos DB instance. You include a valid endpoint and valid authorization key to an appSettings.json file in the code project. You are evaluating the following application code: (Line number are included for reference only.). Question 3: Container2 will contain one item.

![Question 70](images/question68_69_70.png)

- [x] Yes.
- [ ] No.


### You develop an Azure solution that uses Cosmos DB. The current Cosmos DB container must be replicated and must use a partition key that is optimized for queries. You need to implement a change feed processor solution. Which change feed processor components should you use?

![Question 71](images/question71.png)

- [ ] Store the data from which the change feed is generated: Host. Coordinate processing of the change feed across multiple workers: Delegate. Use the change feed processor to listen for changes: Lease container. Handle each batch of changes: Monitored container.
- [ ] Store the data from which the change feed is generated: Lease container. Coordinate processing of the change feed across multiple workers: Host. Use the change feed processor to listen for changes: Delegate. Handle each batch of changes: Monitored container.
- [ ] Store the data from which the change feed is generated: Delegate. Coordinate processing of the change feed across multiple workers: Monitored container. Use the change feed processor to listen for changes: Lease container. Handle each batch of changes: Host.
- [x] Store the data from which the change feed is generated: Monitored container. Coordinate processing of the change feed across multiple workers: Lease container. Use the change feed processor to listen for changes: Host. Handle each batch of changes: Delegate.


### You develop a web application. You need to register the application with an active Azure Active Directory (Azure AD) tenant. Which three actions should you perform in sequence?

![Question 72](images/question72.jpg)

- [ ] Box 1: Select Manifest from the middle-tier service registration. Box 2: Add a Cryptographic key. Box 3: In App Registrations, select New registration.
- [ ] Box 1: In App Registrations, select New registration. Box 2: Select the Azure AD instance. Box 3: Select Manifest from the middle-tier service registration.
- [x] Box 1: In App Registrations, select New registration. Box 2: Select the Azure AD instance. Box 3: Create a new application and provide the name, account type, and redirect URI.
- [ ] Box 1: In Enterprise Applications, select New application. Box 2: In App Registrations, select New registration. Box 3: Select the Azure AD instance.


### You have a new Azure subscription. You are developing an internal website for employees to view sensitive data. The website uses Azure Active Directory (Azure AD) for authentication. You need to implement multifactor authentication for the website. Which two actions should you perform?

- [ ] Configure the website to use Azure AD B2C.
- [x] MFA Enabled by conditional access policy.
- [x] In Azure AD, create a new conditional access policy.
- [ ] Upgrade to Azure AD Premium.
- [ ] In Azure AD, enable application proxy.
- [ ] In Azure AD conditional access, enable the baseline policy.


### You are developing a Java application that uses Cassandra to store key and value data. You plan to use a new Azure Cosmos DB resource and the Cassandra API in the application. You create an Azure Active Directory (Azure AD) group named Cosmos DB Creators to enable provisioning of Azure Cosmos accounts, databases, and containers. The Azure AD group must not be able to access the keys that are required to access the data. You need to restrict access to the Azure AD group. Which role-based access control should you use?

- [ ] DocumentDB Accounts Contributor.
- [ ] Cosmos Backup Operator.
- [x] Cosmos DB Operator.
- [ ] Cosmos DB Account Reader.


### You are developing a website that will run as an Azure Web App. Users will authenticate by using their Azure Active Directory (Azure AD) credentials. You plan to assign users one of the following permission levels for the website: admin, normal, and reader. A user's Azure AD group membership must be used to determine the permission level. You need to configure authorization. Solution: Configure the Azure Web App for the website to allow only authenticated requests and require Azure AD log on. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a website that will run as an Azure Web App. Users will authenticate by using their Azure Active Directory (Azure AD) credentials. You plan to assign users one of the following permission levels for the website: admin, normal, and reader. A user's Azure AD group membership must be used to determine the permission level. You need to configure authorization. Solution: Create a new Azure AD application. In the application's manifest, set value of the groupMembershipClaims option to All. In the website, use the value of the groups claim from the JWT for the user to determine permissions. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing a website that will run as an Azure Web App. Users will authenticate by using their Azure Active Directory (Azure AD) credentials. You plan to assign users one of the following permission levels for the website: admin, normal, and reader. A user's Azure AD group membership must be used to determine the permission level. You need to configure authorization. Solution: Create a new Azure AD application. In the application's manifest, define application roles that match the required permission levels for the application. Assign the appropriate Azure AD group to each role. In the website, use the value of the roles claim from the JWT for the user to determine permissions. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing an application to securely transfer data between on-premises file systems and Azure Blob storage. The application stores keys, secrets, and certificates in Azure Key Vault. The application uses the Azure Key Vault APIs. The application must allow recovery of an accidental deletion of the key vault or key vault objects. Key vault objects must be retained for 90 days after deletion. You need to protect the key vault and key vault objects. Which Azure Key Vault feature should you use?

![Question 78](images/question78.png)

- [x] Enable retention period and accidental deletion: Soft delete. Enforce retention period and accidental deletion: Purge protection.
- [ ] Enable retention period and accidental deletion: Access policy. Enforce retention period and accidental deletion: Soft delete.
- [ ] Enable retention period and accidental deletion: Shared access signature. Enforce retention period and accidental deletion: Pure protection.
- [ ] Enable retention period and accidental deletion: Soft delete. Enforce retention period and accidental deletion: Shared access signature.


### You provide an Azure API Management managed web service to clients. The back-end web service implements HTTP Strict Transport Security (HSTS). Every request to the backend service must include a valid HTTP authorization header. You need to configure the Azure API Management instance with an authentication policy. Which two policies can you use?

- [x] Basic Authentication.
- [ ] Digest Authentication.
- [x] Certificate Authentication.
- [ ] OAuth Client Credential Grant.


### You are developing an ASP.NET Core website that can be used to manage photographs which are stored in Azure Blob Storage containers. Users of the website authenticate by using their Azure Active Directory (Azure AD) credentials. You implement role-based access control (RBAC) role permissions on the containers that store photographs. You assign users to RBAC roles. You need to configure the website's Azure AD Application so that user's permissions can be used with the Azure Blob containers. How should you configure the application?

![Question 80](images/question80.png)

- [ ] Azure Storage Permission: client_id. Azure Storage Type: application. Microsoft Graph Type: user_impersonation.
- [ ] Azure Storage Permission: client_id. Azure Storage Type: profile. Microsoft Graph Type: application.
- [x] Azure Storage Permission: user_impersonation. Azure Storage Type: delegated. Microsoft Graph Type: delegated.
- [ ] Azure Storage Permission: user_impersonation. Azure Storage Type: delegated. Microsoft Graph Type: profile.


### You are developing an ASP.NET Core app that includes feature flags which are managed by Azure App Configuration. You create an Azure App Configuration store named AppFeatureFlagStore that contains a feature flag named Export. You need to update the app to meet the following requirements: Use the Export feature in the app without requiring a restart of the app. Validate users before users are allowed access to secure resources. Permit users to access secure resources. How should you complete the code segment?

![Question 81](images/question81.png)

- [ ] Box 1: UseSession. Box 2: UseCookiePolicy. Box 3: UseStaticFiles.
- [ ] Box 1: UseAuthentication. Box 2: UseAuthorization. Box 3: UseStaticFiles.
- [ ] Box 1: UseCookiePolicy. Box 2: UseHttpsRedirection. Box 3: UseCors.
- [x] Box 1: UseAuthentication. Box 2: UseAuthorization. Box 3: UseAzureAppConfiguration.


### You have an application that includes an Azure Web app and several Azure Function apps. Application secrets including connection strings and certificates are stored in Azure Key Vault. Secrets must not be stored in the application or application runtime environment. Changes to Azure Active Directory (Azure AD) must be minimized. You need to design the approach to loading application secrets. What should you do?

- [ ] Create a single user-assigned Managed Identity with permission to access Key Vault and configure each App Service to use that Managed Identity.
- [ ] Create a single Azure AD Service Principal with permission to access Key Vault and use a client secret from within the App Services to access Key Vault.
- [x] Create a system assigned Managed Identity in each App Service with permission to access Key Vault.
- [ ] Create an Azure AD Service Principal with Permissions to access Key Vault for each App Service and use a certificate from within the App Services to access Key Vault.


### You are developing a medical records document management website. The website is used to store scanned copies of patient intake forms. If the stored intake forms are downloaded from storage by a third party, the contents of the forms must not be compromised. You need to store the intake forms according to the requirements. Solution: 1. Create an Azure Key Vault key named skey. 2. Encrypt the intake forms using the public key portion of skey. 3. Store the encrypted data in Azure Blob storage. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing a medical records document management website. The website is used to store scanned copies of patient intake forms. If the stored intake forms are downloaded from storage by a third party, the contents of the forms must not be compromised. You need to store the intake forms according to the requirements. Solution: 1. Create an Azure Cosmos DB database with Storage Service Encryption enabled. 2. Store the intake forms in the Azure Cosmos DB database. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a medical records document management website. The website is used to store scanned copies of patient intake forms. If the stored intake forms are downloaded from storage by a third party, the contents of the forms must not be compromised. You need to store the intake forms according to the requirements. Solution: Store the intake forms as Azure Key Vault secrets. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You plan to deploy a new application to a Linux virtual machine (VM) that is hosted in Azure. The entire VM must be secured at rest by using industry-standard encryption technology to address organizational security and compliance requirements. You need to configure Azure Disk Encryption for the VM. How should you complete the Azure CLI commands?

![Question 86](images/question86.jpg)

- [x] Box 1: keyvault. Box 2: keyvault key. Box 3: vm. Box 4: vm encryption. Box 5: all.
- [ ] Box 1: vm. Box 2: vm encryption. Box 3: keyvault key. Box 4: keyvault. Box 5: data.
- [ ] Box 1: vm encryption. Box 2: vm. Box 3: keyvault. Box 4: keyvault key. Box 5: all.
- [ ] Box 1: keyvault key. Box 2: keyvault. Box 3: vm encryption. Box 4: vm. Box 5: os.


### Your company is developing an Azure API hosted in Azure. You need to implement authentication for the Azure API to access other Azure resources. You have the following requirements: All API calls must be authenticated. Callers to the API must not send credentials to the API. Which authentication mechanism should you use?

- [ ] Basic.
- [ ] Anonymous.
- [x] Managed identity.
- [ ] Client certificate.


### You are using Azure Front Door Service. You are expecting inbound files to be compressed by using Brotli compression. You discover that inbound XML files are not compressed. The files are 9 megabytes (MB) in size. You need to determine the root cause for the issue. Question 1: The file MIME type is supported by the service.

- [ ] Yes.
- [x] No.


### You are using Azure Front Door Service. You are expecting inbound files to be compressed by using Brotli compression. You discover that inbound XML files are not compressed. The files are 9 megabytes (MB) in size. You need to determine the root cause for the issue. Question 2: Edge nodes must be purged of all cache assets.

- [x] Yes.
- [ ] No.


### You are using Azure Front Door Service. You are expecting inbound files to be compressed by using Brotli compression. You discover that inbound XML files are not compressed. The files are 9 megabytes (MB) in size. You need to determine the root cause for the issue. Question 3: The compression type is supported.

- [x] Yes.
- [ ] No.


### You are developing an application. You have an Azure user account that has access to two subscriptions. You need to retrieve a storage account key secret from Azure Key Vault. In which order should you arrange the PowerShell commands to develop the solution?

![Question 91](images/question91.png)

- [ ] Box 1: Get-AzSubscription. Box 2: Set-AzContext -SubscriptionId $subscriptionID. Box 3: Get-AzStorageAccountKey -ResourceGroupName $resGroup -Name $storAcct. Box 4: Get-AzKeyVaultSecret -VaultName $vaultName. Box 5: $secretvalue = ConvertTo-SecureString $storAcctkey -AsPlainText -Force Set-AzKeyVaultSecret -VaultName $vaultName -Name $secretName -SecretValue $secretvalue.
- [ ] Box 1: Set-AzContext -SubscriptionId $subscriptionID. Box 2: Get-AzStorageAccountKey -ResourceGroupName $resGroup -Name $storAcct. Box 3: Get-AzKeyVaultSecret -VaultName $vaultName. Box 4: $secretvalue = ConvertTo-SecureString $storAcctkey -AsPlainText -Force Set-AzKeyVaultSecret -VaultName $vaultName -Name $secretName -SecretValue $secretvalue. Box 5: Get-AzSubscription.
- [x] Box 1: Get-AzSubscription. Box 2: Set-AzContext -SubscriptionId $subscriptionID. Box 3: Get-AzStorageAccountKey -ResourceGroupName $resGroup -Name $storAcct. Box 4: $secretvalue = ConvertTo-SecureString $storAcctkey -AsPlainText -Force Set-AzKeyVaultSecret -VaultName $vaultName -Name $secretName -SecretValue $secretvalue. Box 5: Get-AzKeyVaultSecret -VaultName $vaultName.
- [ ] Box 1: Get-AzKeyVaultSecret -VaultName $vaultName. Box 2: Get-AzSubscription. Box 3: Set-AzContext -SubscriptionId $subscriptionID. Box 4: Get-AzStorageAccountKey -ResourceGroupName $resGroup -Name $storAcct. Box 5: $secretvalue = ConvertTo-SecureString $storAcctkey -AsPlainText -Force Set-AzKeyVaultSecret -VaultName $vaultName -Name $secretName -SecretValue $secretvalue.


### You develop Azure solutions. You must grant a virtual machine (VM) access to specific resource groups in Azure Resource Manager. You need to obtain an Azure Resource Manager access token. Solution: Use an X.509 certificate to authenticate the VM with Azure Resource Manager. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop Azure solutions. You must grant a virtual machine (VM) access to specific resource groups in Azure Resource Manager. You need to obtain an Azure Resource Manager access token. Solution: Use the Reader role-based access control (RBAC) role to authenticate the VM with Azure Resource Manager. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are building a website that is used to review restaurants. The website will use an Azure CDN to improve performance and add functionality to requests. You build and deploy a mobile app for Apple iPhones. Whenever a user accesses the website from an iPhone, the user must be redirected to the app store. You need to implement an Azure CDN rule that ensures that iPhone users are redirected to the app store. How should you complete the Azure Resource Manager template?

![Question 94](images/question94.png)

- [ ] Box 1: iOS. Box 2: DeliveryRulelsDeviceConditionParameters. Box 3: HTTP_USER_AGENT. Box 4: DeliveryRuleRequestHeaderConditionParameters. Box 5: iOS.
- [x] Box 1: Mobile. Box 2: DeliveryRulelsDeviceConditionParameters. Box 3: HTTP_USER_AGENT. Box 4: DeliveryRuleRequestHeaderConditionParameters. Box 5: iPhone.
- [ ] Box 1: Desktop. Box 2: DeliveryRuleCookiesConditionParameters. Box 3: PRAGMA. Box 4: DeliveryRulelsDeviceConditionParameters. Box 5: Desktop.
- [ ] Box 1: iOS. Box 2: DeliveryRulelsDeviceConditionParameters. Box 3: FROM. Box 4: DeliveryRulePostArgsConditionParameters. Box 5: Mobile.


### You are developing a website that will run as an Azure Web App. Users will authenticate by using their Azure Active Directory (Azure AD) credentials. You plan to assign users one of the following permission levels for the website: admin, normal, and reader. A user's Azure AD group membership must be used to determine the permission level. You need to configure authorization. Solution: Configure and use Integrated Windows Authentication in the website. In the website, query Microsoft Graph API to load the group to which the user is a member. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop Azure solutions. You must grant a virtual machine (VM) access to specific resource groups in Azure Resource Manager. You need to obtain an Azure Resource Manager access token. Solution: Run the Invoke-RestMethod cmdlet to make a request to the local managed identity for Azure resources endpoint. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### Your company's Azure subscription includes an Azure Log Analytics workspace. Your company has a hundred on-premises servers that run either Windows Server 2012 R2 or Windows Server 2016, and is linked to the Azure Log Analytics workspace. The Azure Log Analytics workspace is set up to gather performance counters associated with security from these linked servers. You must configure alerts based on the information gathered by the Azure Log Analytics workspace. You have to make sure that alert rules allow for dimensions, and that alert creation time should be kept to a minimum. Furthermore, a single alert notification must be created when the alert is created and when the alert is resolved. You need to make use of the necessary signal type when creating the alert rules. Which of the following is the option you should use?

- [ ] The Activity log signal type.
- [ ] The Application Log signal type.
- [x] The Metric signal type.
- [ ] The Audit Log signal type.


### You are developing a .NET Core MVC application that allows customers to research independent holiday accommodation providers. You want to implement Azure Search to allow the application to search the index by using various criteria to locate documents related to accommodation. You want the application to allow customers to search the index by using regular expressions. What should you do?

- [ ] Configure the SearchMode property of the SearchParameters class.
- [x] Configure the QueryType property of the SearchParameters class.
- [ ] Configure the Facets property of the SearchParameters class.
- [ ] Configure the Filter property of the SearchParameters class.


### You are a developer at your company. You need to update the definitions for an existing Logic App. What should you use?

- [ ] The Enterprise Integration Pack (EIP).
- [x] The Logic App Code View.
- [ ] The API Connections.
- [ ] The Logic Apps Designer.


### The cluster uses Azure Monitor for containers to monitor the cluster. The application has sticky sessions enabled on the ingress controller. Some customers report a large number of errors in the application over the last 24 hours. You need to determine on which virtual machines (VMs) the errors are occurring. How should you complete the Azure Monitor query?

![Question 100](images/question100.png)

- [x] Box 1: ago(1d). Box 2: distinct ContainerlD. Box 3: where ContainerlD in (ContainerIDs). Box 4: summarize count() by Computer.
- [ ] Box 1: date(now() - 1d). Box 2: sample ContainerlD. Box 3: where ContainerlD in (ContainerIDs). Box 4: partition count() by Computer.
- [ ] Box 1: ago(1d). Box 2: distinct ContainerlD. Box 3: join ContainerlD = = ContainerlDs.ContainerlD. Box 4: summarize by Computer.
- [ ] Box 1: totimespan(1d). Box 2: top ContainerlD. Box 3: fork containerIDs. Box 4: project by Computer.


### You plan to deploy a web app to App Service on Linux. You create an App Service plan. You create and push a custom Docker image that contains the web app to Azure Container Registry. You need to access the console logs generated from inside the container in real-time. How should you complete the Azure CLI command?

![Question 101](images/question101.png)

- [x] Box 1: config. Box 2: --docker-container-logging. Box 3: webapp. Box 4: tail.
- [ ] Box 1: tail. Box 2: --web-server-logging Box 3: aks Box 4: show.
- [ ] Box 1: show. Box 2: --web-server-logging. Box 3: acr. Box 4: config.
- [ ] Box 1: config. Box 2: --application-logging. Box 3: webapp. Box 4: show.


### You develop an app that allows users to upload photos and videos to Azure storage. The app uses a storage REST API call to upload the media to a blob storage account named Account1. You have blob storage containers named Container1 and Container2. Uploading of videos occurs on an irregular basis. You need to copy specific blobs from Container1 to Container2 when a new video is uploaded. What should you do?

- [ ] Copy blobs to Container2 by using the Put Blob operation of the Blob Service REST API.
- [x] Create an Event Grid topic that uses the Start-AzureStorageBlobCopy cmdlet.
- [ ] Use AzCopy with the Snapshot switch to copy blobs to Container2.
- [ ] Download the blob to a virtual machine and then upload the blob to Container2.


### A web service provides customer summary information for e-commerce partners. The web service is implemented as an Azure Function app with an HTTP trigger. Access to the API is provided by an Azure API Management instance. The API Management instance is configured in consumption plan mode. All API calls are authenticated by using OAuth. API calls must be cached. Customers must not be able to view cached data for other customers. You need to configure API Management policies for caching. How should you complete the policy statement?

![Question 103](images/question103.jpg)

- [x] caching-type: Internal. downstream-caching-type: Private. vary-by-header: Authorization.
- [ ] caching-type: Public. downstream-caching-type: Expect. vary-by-header: Private.
- [ ] caching-type: Internal. downstream-caching-type: External. vary-by-header: Authorization.
- [ ] caching-type: External. downstream-caching-type: Private. vary-by-header: Authorization.


### You are developing an ASP.NET Core website that uses Azure FrontDoor. The website is used to build custom weather data sets for researchers. Data sets are downloaded by users as Comma Separated Value (CSV) files. The data is refreshed every 10 hours. Specific files must be purged from the FrontDoor cache based upon Response Header values. You need to purge individual assets from the Front Door cache. Which type of cache purge should you use?

- [x] single path.
- [ ] wildcard.
- [ ] root domain.


### Contoso, Ltd. provides an API to customers by using Azure API Management (APIM). The API authorizes users with a JWT token. You must implement response caching for the APIM gateway. The caching mechanism must detect the user ID of the client that accesses data for a given location and cache the response for that user ID. You need to add the following policies to the policies file: a set-variable policy to store the detected user identity a cache-lookup-value policy a cache-store-value policy a find-and-replace policy to update the response body with the user profile information To which policy section should you add the policies?

![Question 105](images/question105.jpg)

- [x] Set-variable: Inbound. Cache-lookup-value: Inbound. Cache-store-value: Outbound. Find-and-replace: Outbound.
- [ ] Set-variable: Outbound. Cache-lookup-value: Inbound. Cache-store-value: Outbound. Find-and-replace: Inbound.
- [ ] Set-variable: Inbound. Cache-lookup-value: Outbound. Cache-store-value: Inbound. Find-and-replace: Outbound.
- [ ] Set-variable: Outbound. Cache-lookup-value: Outbound. Cache-store-value: Inbound. Find-and-replace: Inbound.


### You are developing an application to retrieve user profile information. The application will use the Microsoft Graph SDK. The app must retrieve user profile information by using a Microsoft Graph API call. You need to call the Microsoft Graph API from the application. In which order should you perform the actions?

![Question 106](images/question106.jpg)

- [x] Box 1: Register the application with the Microsoft identity platform. Box 2: Build a client by using the client app ID. Box 3: Create an authentication provider. Box 4: Create a new instance of the GraphServiceClient. Box 5: Invoke the request to the Microsoft Graph API.
- [ ] Box 1: Invoke the request to the Microsoft Graph API. Box 2: Create an authentication provider. Box 3: Register the application with the Microsoft identity platform. Box 4: Build a client by using the client app ID. Box 5: Create a new instance of the GraphServiceClient.
- [ ] Box 1: Build a client by using the client app ID. Box 2: Register the application with the Microsoft identity platform. Box 3: Create an authentication provider. Box 4: Create a new instance of the GraphServiceClient. Box 5: Invoke the request to the Microsoft Graph API.
- [ ] Box 1: Register the application with the Microsoft identity platform. Box 2: Build a client by using the client app ID. Box 3: Invoke the request to the Microsoft Graph API. Box 4: Create a new instance of the GraphServiceClient. Box 5: Create an authentication provider. Graph API.


### You develop and deploy an Azure Logic App that calls an Azure Function app. The Azure Function App includes an OpenAPI (Swagger) definition and uses an Azure Blob storage account. All resources are secured by using Azure Active Directory (Azure AD). The Logic App must use Azure Monitor logs to record and store information about runtime data and events. The logs must be stored in the Azure Blob storage account. You need to set up Azure Monitor logs and collect diagnostics data for the Azure Logic App. Which three actions should you perform in sequence?

![Question 107](images/question107.png)

- [x] Box 1: Create a Log Analytics workspace. Box 2: Install the Logic Apps Management solution. Box 3: Add a diagnostic setting to the Azure Logic App.
- [ ] Box 1: Install the Logic Apps Management solution. Box 2: Add a diagnostic setting to the Azure Function App. Box 3: Create action groups and alert rules.
- [ ] Box 1: Add a diagnostic setting to the Azure Function App. Box 2: Create a Log Analytics workspace. Box 3: Create action groups and alert rules.
- [ ] Box 1: Create a Log Analytics workspace. Box 2: Create action groups and alert rules. Box 3: Add a diagnostic setting to the Azure Function App.


### You develop an application. You plan to host the application on a set of virtual machines (VMs) in Azure. You need to configure Azure Monitor to collect logs from the application. Which four actions should you perform in sequence?

![Question 108](images/question108.png)

- [x] Box 1: Create a Log Analytics workspace. Box 2: Add a VMInsights solution. Box 3: Install agents on the VM and VM scale set to be monitored. Box 4: Create an Application Insights resource.
- [ ] Box 1: Add a VMInsights solution. Box 2: Create a Log Analytics workspace. Box 3: AInstall agents on the VM and VM scale set to be monitored. Box 4: Create an Application Insights resource.
- [ ] Box 1: Create an Application Insights resource. Box 2: Add a VMInsights solution. Box 3: AInstall agents on the VM and VM scale set to be monitored. Box 4: Create a Log Analytics workspace.
- [ ] Box 1: Create a Log Analytics workspace. Box 2: Add a VMInsights solution. Box 3: Create an Application Insights resource. Box 4: Install agents on the VM and VM scale set to be monitored.


### You have an application that provides weather forecasting data to external partners. You use Azure API Management to publish APIs. You must change the behavior of the API to meet the following requirements: Support alternative input parameters. Remove formatting text from responses. Provide additional context to back-end services. Which types of policies should you implement?

![Question 109](images/question109.png)

- [x] Rewrite the request URL to match to the format expected by the web service: Inbound. Remove formatting text from responses: Outbound. Forward the user ID that is associated with the subscription key for the original request to the back-end service: Inbound.
- [ ] Rewrite the request URL to match to the format expected by the web service: Inbound. Remove formatting text from responses: Outbound. Forward the user ID that is associated with the subscription key for the original request to the back-end service: Backend.
- [ ] Rewrite the request URL to match to the format expected by the web service: Inbound. Remove formatting text from responses: Backend. Forward the user ID that is associated with the subscription key for the original request to the back-end service: Inbound.
- [ ] Rewrite the request URL to match to the format expected by the web service: Backend. Remove formatting text from responses: Backend. Forward the user ID that is associated with the subscription key for the original request to the back-end service: Inbound.


### Your company is developing an Azure API. You need to implement authentication for the Azure API. You have the following requirements: All API calls must be secure. Callers to the API must not send credentials to the API. Which authentication mechanism should you use?

- [ ] Basic.
- [ ] Anonymous.
- [x] Managed identity.
- [ ] Client certificate.


### You are a developer for a SaaS company that offers many web services. All web services for the company must meet the following requirements: Use API Management to access the services Use OpenID Connect for authentication Prevent anonymous usage A recent security audit found that several web services can be called without any authentication. Which API Management policy should you implement?

- [ ] jsonp.
- [ ] authentication-certificate.
- [ ] check-header.
- [x] validate-jwt.


### You are developing an Azure App Service REST API. The API must be called by an Azure App Service web app. The API must retrieve and update user profile information stored in Azure Active Directory (Azure AD). You need to configure the API to make the updates. Which two tools should you use?

- [x] Microsoft Graph API.
- [ ] Microsoft Authentication Library (MSAL).
- [x] Azure API Management.
- [ ] Microsoft Azure Security Center.
- [ ] Microsoft Azure Key Vault SDK.


### You develop a REST API. You implement a user delegation SAS token to communicate with Azure Blob storage. The token is compromised. You need to revoke the token. What are two possible ways to achieve this goal?

- [x] Revoke the delegation key.
- [x] Delete the stored access policy.
- [ ] Regenerate the account key.
- [ ] Remove the role assignment for the security principle.


### You are developing an Azure-hosted application that must use an on-premises hardware security module (HSM) key. The key must be transferred to your existing Azure Key Vault by using the Bring Your Own Key (BYOK) process. You need to securely transfer the key to Azure Key Vault. Which four actions should you perform in sequence?

![Question 114](images/question114.jpeg)

- [ ] Box 1: Create a custom policy definition in Azure Policy. Box 2: Generate a Key Exchange Key (KEK). Box 3: Retrieve the Key Exchange Key (KEK) public key. Box 4: Run the az keyvault key import command.
- [ ] Box 1: Create a custom policy definition in Azure Policy. Box 2: Retrieve the Key Exchange Key (KEK) public key. Box 3: Generate a key transfer blob file by using the HSM vendor-provided tool. Box 4: Run the az keyvault key import command.
- [ ] Box 1: Generate a Key Exchange Key (KEK). Box 2: Retrieve the Key Exchange Key (KEK) public key. Box 3: Generate a key transfer blob file by using the HSM vendor-provided tool. Box 4: Run the az keyvault key restore command.
- [x] Box 1: Generate a Key Exchange Key (KEK). Box 2: Retrieve the Key Exchange Key (KEK) public key. Box 3: Generate a key transfer blob file by using the HSM vendor-provided tool. Box 4: Run the az keyvault key import command.


### You develop and deploy an Azure Logic app that calls an Azure Function app. The Azure Function app includes an OpenAPI (Swagger) definition and uses an Azure Blob storage account. All resources are secured by using Azure Active Directory (Azure AD). The Azure Logic app must securely access the Azure Blob storage account. Azure AD resources must remain if the Azure Logic app is deleted. You need to secure the Azure Logic app. What should you do?

- [x] Create a user-assigned managed identity and assign role-based access controls.
- [ ] Create an Azure AD custom role and assign the role to the Azure Blob storage account.
- [ ] Create an Azure Key Vault and issue a client certificate.
- [ ] Create a system-assigned managed identity and issue a client certificate.
- [ ] Create an Azure AD custom role and assign role-based access controls.


### You manage several existing Logic Apps. You need to change definitions, add new logic, and optimize these apps on a regular basis. What should you use?

![Question 116](images/question116.jpg)

- [x] Edit B2B Workflows: Enterprise Integration Pack. Edit definitions in JSON: Code View Editor. Visually add functionality: Logic Apps Designer.
- [ ] Edit B2B Workflows: Logic Apps Designer. Edit definitions in JSON: Enterprise Integration Pack. Visually add functionality: Code View Editor.
- [ ] Edit B2B Workflows: Code View Editor. Edit definitions in JSON: Logic Apps Designer. Visually add functionality: Enterprise Integration Pack.
- [ ] Edit B2B Workflows: Enterprise Integration Pack. Edit definitions in JSON: Code View Editor. Visually add functionality: Code View Editor.


### You are developing a solution that will use a multi-partitioned Azure Cosmos DB database. You plan to use the latest Azure Cosmos DB SDK for development. The solution must meet the following requirements: Send insert and update operations to an Azure Blob storage account. Process changes to all partitions immediately. Allow parallelization of change processing. You need to process the Azure Cosmos DB operations. What are two possible ways to achieve this goal?

- [ ] Create an Azure App Service API and implement the change feed estimator of the SDK. Scale the API by using multiple Azure App Service instances.
- [ ] Create a background job in an Azure Kubernetes Service and implement the change feed feature of the SDK.
- [x] Create an Azure Function to use a trigger for Azure Cosmos DB. Configure the trigger to connect to the container.
- [x] Create an Azure Function that uses a FeedIterator object that processes the change feed by using the pull model on the container. Use a FeedRange object to parallelize the processing of the change feed across multiple functions.


### You are developing an application that uses Azure Storage Queues. You have the following code. Question 1: The code configures the lock duration for the queue.

![Question 118](images/question118_119_120.jpg)

- [ ] Yes.
- [x] No.


### You are developing an application that uses Azure Storage Queues. You have the following code. Question 2: The last message read remains in the queue after the code runs.

![Question 119](images/question118_119_120.jpg)

- [x] Yes.
- [ ] No.


### You are developing an application that uses Azure Storage Queues. You have the following code. Question 3: The storage queue remains in the storage account after the code runs.

![Question 120](images/question118_119_120.jpg)

- [x] Yes.
- [ ] No.


### You develop software solutions for a mobile delivery service. You are developing a mobile app that users can use to order from a restaurant in their area. The app uses the following workflow: 1. A driver selects the restaurants for which they will deliver orders. 2. Orders are sent to all available drivers in an area. 3. Only orders for the selected restaurants will appear for the driver. 4. The first driver to accept an order removes it from the list of available orders. You need to implement an Azure Service Bus solution. Which three actions should you perform in sequence?

![Question 121](images/question121.png)

- [x] Box 1: Create a single Service Bus topic. Box 2: Create a Service Bus Namespace for each restaurat for which a driver can receive messages. Box 3: Create a Service Bus subscription for each restaurant for which a driver can receive orders.
- [ ] Box 1: Create a Service Bus subscription for each restaurant for which a driver can receive orders. Box 2: Create a Service Bus topic for each restaurant. Box 3: Create a Service Bus Namespace for each.
- [ ] Box 1: Create a single Service Bus topic. Box 2: Create a Service Bus subscription for each restaurant for which a driver can receive orders. Box 3: Create a single Service Bus topic.
- [ ] Box 1: Create a single Service Bus topic. Box 2: Create a Service Bus Namespace for each restaurat for which a driver can receive messages. Box 3: Create a Service Bus Namespace for each.


### You develop a news and blog content app for Windows devices. A notification must arrive on a user's device when there is a new article available for them to view. You need to implement push notifications. How should you complete the code segment?

![Question 122](images/question122.png)

- [x] Box 1: NotificationHubClient. Box 2: NotificationHubClient. Box 3: CreateClientFromConnectionString. Box 4: SendWindowsNativeNotificationAsync.
- [ ] Box 1: NotificationHubJob. Box 2: NotificationHubJob. Box 3: Patchlinstallation. Box 4: SendWindowsNativeNotificationAsync.
- [ ] Box 1: NotificationHubClientSettings. Box 2: NotificationHubClientSettings. Box 3: CreateOrUpdatelnstallation. Box 4: ScheduleNotificationAsync.
- [ ] Box 1: NotificationHubClientSettings. Box 2: NotificationDetails. Box 3: CreateOrUpdatelnstallation. Box 4: SendWindowsNativeNotificationAsync.


### You are developing an Azure messaging solution. You need to ensure that the solution meets the following requirements: Provide transactional support. Provide duplicate detection. Store the messages for an unlimited period of time. Which two technologies will meet the requirements?

- [x] Azure Service Bus Topic.
- [x] Azure Service Bus Queue.
- [ ] Azure Storage Queue.
- [ ] Azure Event Hub.


### You develop a gateway solution for a public facing news API. The news API back end is implemented as a RESTful service and hosted in an Azure App Service instance. You need to configure back-end authentication for the API Management service instance. Which target and gateway credential type should you use?

![Question 124](images/question124.jpg)

- [x] Target: Azure Resource. Gateway credentials: Client cert.
- [ ] Target: Client cert. Gateway credentials: Basic.
- [ ] Target: Azure Resource. Gateway credentials: Basic.
- [ ] Target: Basic. Gateway credentials: HTTP(s) endpoint.


### You are creating an app that uses Event Grid to connect with other services. Your app's event data will be sent to a serverless function that checks compliance. This function is maintained by your company. You write a new event subscription at the scope of your resource. The event must be invalidated after a specific period of time. You need to configure Event Grid. What should you do?

![Question 125](images/question125.jpg)

- [x] WebHook event delivery: SAS tokens. Topic publishing: ValidationCode handshake.
- [ ] WebHook event delivery: Key authentication. Topic publishing: ValidationCode handshake.
- [ ] WebHook event delivery: Management Access Control. Topic publishing: ValidationURL handshake.
- [ ] WebHook event delivery: SAS tokens. Topic publishing: ValidationURL handshake.


### You are working for Contoso, Ltd. You define an API Policy object by using the following XML markup. Question 1: The XML segment belongs in the <inbound> section of the policy.

![Question 126](images/question126_127_128.png)

- [x] Yes.
- [ ] No.


### You are working for Contoso, Ltd. You define an API Policy object by using the following XML markup. Question 2: If the body size is >256k, an error will occur.

![Question 127](images/question126_127_128.png)

- [ ] Yes.
- [x] No.


### You are working for Contoso, Ltd. You define an API Policy object by using the following XML markup. Question 3: If the request is <http://contoso.com/api/9.2/>, the policy will retain the higher version.

![Question 128](images/question126_127_128.png)

- [ ] Yes.
- [x] No.


### You develop a gateway solution for a public facing news API. The news API back end is implemented as a RESTful service and uses an OpenAPI specification. You need to ensure that you can access the news API by using an Azure API Management service instance. Which Azure PowerShell command should you run?

- [x] Import-AzureRmApiManagementApi -Context $ApiMgmtContext -SpecificationFormat 'Swagger' -SpecificationPath $SwaggerPath -Path $Path.
- [ ] New-AzureRmApiManagementBackend -Context $ApiMgmtContext-Url $Url -Protocol http.
- [ ] New-AzureRmApiManagement -ResourceGroupName $ResourceGroup -Name $Name 'Location $Location -Organization $Org -AdminEmail $AdminEmail.
- [ ] New-AzureRmApiManagementBackendProxy -Url $ApiUrl.


### You are developing an Azure function that connects to an Azure SQL Database instance. The function is triggered by an Azure Storage queue. You receive reports of numerous System.InvalidOperationExceptions with the following message: 'Timeout expired. The timeout period elapsed prior to obtaining a connection from the pool. This may have occurred because all pooled connections were in use and max pool size was reached.' You need to prevent the exception. What should you do?

- [ ] In the host.json file, decrease the value of the batchSize option.
- [ ] Convert the trigger to Azure Event Hub.
- [x] Convert the Azure Function to the Premium plan.
- [ ] In the function.json file, change the value of the type option to queueScaling.


### You are developing a REST web service. Customers will access the service by using an Azure API Management instance. The web service does not correctly handle conflicts. Instead of returning an HTTP status code of 409, the service returns a status code of 500. The body of the status message contains only the word conflict. You need to ensure that conflicts produce the correct response. How should you complete the policy?

![Question 131](images/question131.png)

- [x] Box 1: on-error. Box 2: context. Box 3: context. Box 4: set-status. Box 5: on-error.
- [ ] Box 1: when-error. Box 2: context. Box 3: server. Box 4: override-status. Box 5:on-error.
- [ ] Box 1: when-error. Box 2: context. Box 3: context. Box 4: set-status. Box 5:on-error.
- [ ] Box 1: on-error. Box 2: context. Box 3: server. Box 4: override-status. Box 5:on-error.


### You are a developer for a Software as a Service (SaaS) company. You develop solutions that provide the ability to send notifications by using Azure Notification Hubs. You need to create sample code that customers can use as a reference for how to send raw notifications to Windows Push Notification Services (WNS) devices. The sample code must not use external packages. How should you complete the code segment?

![Question 132](images/question132.jpg)

- [x] Box 1: windows. Box 2: application/octet-stream.
- [ ] Box 1: windowsphone. Box 2: raw.
- [ ] Box 1: windows. Box 2: application/json.
- [ ] Box 1: windowsphone. Box 2: application/xml.


### You develop and deploy an ASP.NET web app to Azure App Service. You use Application Insights telemetry to monitor the app. You must test the app to ensure that the app is available and responsive from various points around the world and at regular intervals. If the app is not responding, you must send an alert to support staff. You need to configure a test for the web app. Which two test types can you use?

- [ ] Integration.
- [x] TrackAvailablity.
- [x] URL ping.
- [ ] Unit.
- [ ] Load.


### You are developing an Azure solution to collect inventory data from thousands of stores located around the world. Each store location will send the inventory data hourly to an Azure Blob storage account for processing. The solution must meet the following requirements: Begin processing when data is saved to Azure Blob storage. Filter data based on store location information. Trigger an Azure Logic App to process the data for output to Azure Cosmos DB. Enable high availability and geographic distribution. Allow 24-hours for retries. Implement an exponential back off data processing. You need to configure the solution. What should you implement?

![Question 134](images/question134.png)

- [ ] Event Source: Azure Event Grid. Event Receiver: Azure Logic App. Event Handler: Azure Service Bus.
- [ ] Event Source: Azure Service Bus. Event Receiver: Azure App Service. Event Handler: Azure Blob Storage.
- [ ] Event Source: Azure Event Grid. Event Receiver: Azure Service Bus. Event Handler: Azure Blob Storage.
- [x] Event Source: Azure Blob Storage. Event Receiver: Azure Event Grid. Event Handler: Azure Logic App.


### Determine whether the solution meets the stated goals. You are developing and deploying several ASP.NET web applications to Azure App Service. You plan to save session state information and HTML output. You must use a storage mechanism with the following requirements: Share session state across all ASP.NET web applications. Support controlled, concurrent access to the same session state data for multiple readers and a single writer. Save full HTTP responses for concurrent requests. You need to store the information. Proposed Solution: Enable Application Request Routing (ARR). Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### Determine whether the solution meets the stated goals. You are developing and deploying several ASP.NET web applications to Azure App Service. You plan to save session state information and HTML output. You must use a storage mechanism with the following requirements: Share session state across all ASP.NET web applications. Support controlled, concurrent access to the same session state data for multiple readers and a single writer. Save full HTTP responses for concurrent requests. You need to store the information. Proposed Solution: Deploy and configure an Azure Database for PostgreSQL. Update the web applications. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### Determine whether the solution meets the stated goals. You are developing and deploying several ASP.NET web applications to Azure App Service. You plan to save session state information and HTML output. You must use a storage mechanism with the following requirements: Share session state across all ASP.NET web applications. Support controlled, concurrent access to the same session state data for multiple readers and a single writer. Save full HTTP responses for concurrent requests. You need to store the information. Proposed Solution: Deploy and configure Azure Cache for Redis. Update the web applications. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### A company is developing a gaming platform. Users can join teams to play online and see leaderboards that include player statistics. The solution includes an entity named Team. You plan to implement an Azure Redis Cache instance to improve the efficiency of data operations for entities that rarely change. You need to invalidate the cache when team data is changed. How should you complete the code?

![Question 138](images/question138.jpg)

- [x] Box 1: IDatabase cache = Connection.GetDatabase(); Box 2: cache.StringSet('Team', '');
- [ ] Box 1: IDatabase cache = Connection.GetDatabase(); Box 2: cache ValueDelete('Team');
- [ ] Box 1: ICache cache = Connection.GetDatabase(); Box 2: cache KeyDelete('Team');
- [ ] Box 1:ICache cache = Connection.GetDatabase(); Box 2: cache StringGet('Team', '');


### A company has multiple warehouses. Each warehouse contains IoT temperature devices which deliver temperature data to an Azure Service Bus queue. You need to send email alerts to facility supervisors immediately if the temperature at a warehouse goes above or below specified threshold temperatures. Which five actions should you perform in sequence?

![Question 139](images/question139.png)

- [x] Box 1: Create a blank Logic app. Box 2: Add a logic app trigger that fires when one or more messages arrive in the queue. Box 3: Add an action that reads IoT temperature data from the Service Bus queue. Box 4: Add a condition that compares the temperature against the upper and lower thresholds. Box 5: Add an action that sends an email to
specified personnel if the temperature is outside of those thresholds.
- [ ] Box 1: Add a trigger that reads IoT temperature data from a Service Bus queue. Box 2: Add a condition that compares the temperature against the upper and lower thresholds. Box 3: Add a logic app action that fires when one or more messages arrive in the queue. Box 4: Create a blank Logic app. Box 5: Add an action that sends an email to specified personnel if the temperature is outside of those thresholds.
- [ ] Box 1: Add a condition that compares the temperature against the upper and lower thresholds. Box 2: Outbound. Box 3: Add a Recurence rigge that schedules the app to run every 15 minutes. Box 4: Add a trigger that reads IoT temperature data from a Service Bus queue. Box 5: Create a blank Logic app.
- [ ] Box 1: Create a blank Logic app. Box 2: Add a logic app action that fires when one or more messages arrive in the queue. Box 3: Add a condition that compares the temperature against the upper and lower thresholds. Box 4: Add an action that reads IoT temperature data from the Service Bus queue. Box 5: Add a condition that compares the temperature against the upper and lower thresholds.


### You are creating a hazard notification system that has a single signaling server which triggers audio and visual alarms to start and stop. You implement Azure Service Bus to publish alarms. Each alarm controller uses Azure Service Bus to receive alarm signals as part of a transaction. Alarm events must be recorded for audit purposes. Each transaction record must include information about the alarm type that was activated. You need to implement a reply trail auditing solution. Which two actions should you perform?

- [x] Assign the value of the hazard message SessionID property to the ReplyToSessionId property.
- [ ] Assign the value of the hazard message MessageId property to the DevileryCount property.
- [ ] Assign the value of the hazard message SessionID property to the SequenceNumber property.
- [x] Assign the value of the hazard message MessageId property to the CorrelationId property.
- [ ] Assign the value of the hazard message SequenceNumber property to the DeliveryCount property.
- [ ] Assign the value of the hazard message MessageId property to the SequenceNumber property.


### You are developing applications for a company. You plan to host the applications on Azure App Services. The company has the following requirements: Every five minutes verify that the websites are responsive. Verify that the websites respond within a specified time threshold. Dependent requests such as images and JavaScript files must load properly. Generate alerts if a website is experiencing issues. If a website fails to load, the system must attempt to reload the site three more times. You need to implement this process with the least amount of effort. What should you do?

- [ ] Create a Selenium web test and configure it to run from your workstation as a scheduled task.
- [x] Set up a URL ping test to query the home page.
- [ ] Create an Azure function to query the home page.
- [ ] Create a multi-step web test to query the home page.
- [ ] Create a Custom Track Availability Test to query the home page.


### You develop and add several functions to an Azure Function app that uses the latest runtime host. The functions contain several REST API endpoints secured by using SSL. The Azure Function app runs in a Consumption plan. You must send an alert when any of the function endpoints are unavailable or responding too slowly. You need to monitor the availability and responsiveness of the functions. What should you do?

- [ ] Create a URL ping test.
- [x] Create a timer triggered function that calls TrackAvailability() and send the results to Application Insights.
- [ ] Create a timer triggered function that calls GetMetric('Request Size') and send the results to Application Insights.
- [ ] Add a new diagnostic setting to the Azure Function app. Enable the FunctionAppLogs and Send to Log Analytics options.


### You are developing an e-commerce solution that uses a microservice architecture. You need to design a communication backplane for communicating transactional messages between various parts of the solution. Messages must be communicated in first-in-first-out (FIFO) order. What should you use?

- [ ] Azure Storage Queue.
- [ ] Azure Event Hub.
- [x] Azure Service Bus.
- [ ] Azure Event Grid.


### You are developing an Azure Service application that processes queue data when it receives a message from a mobile application. Messages may not be sent to the service consistently. You have the following requirements: Queue size must not grow larger than 80 gigabytes (GB). Use first-in-first-out (FIFO) ordering of messages. Minimize Azure costs. You need to implement the messaging solution. Solution: Use the .Net API to add a message to an Azure Service Bus Queue from the mobile application. Create an Azure Function App that uses an Azure Service Bus Queue trigger. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing an Azure solution to collect point-of-sale (POS) device data from 2,000 stores located throughout the world. A single device can produce 2 megabytes (MB) of data every 24 hours. Each store location has one to five devices that send data. You must store the device data in Azure Blob storage. Device data must be correlated based on a device identifier. Additional stores are expected to open in the future. You need to implement a solution to receive the device data. Solution: Provision an Azure Notification Hub. Register all devices with the hub. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing an Azure solution to collect point-of-sale (POS) device data from 2,000 stores located throughout the world. A single device can produce 2 megabytes (MB) of data every 24 hours. Each store location has one to five devices that send data. You must store the device data in Azure Blob storage. Device data must be correlated based on a device identifier. Additional stores are expected to open in the future. You need to implement a solution to receive the device data. Solution: Provision an Azure Service Bus. Configure a topic to receive the device data by using a correlation filter. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing an Azure solution to collect point-of-sale (POS) device data from 2,000 stores located throughout the world. A single device can produce 2 megabytes (MB) of data every 24 hours. Each store location has one to five devices that send data. You must store the device data in Azure Blob storage. Device data must be correlated based on a device identifier. Additional stores are expected to open in the future. You need to implement a solution to receive the device data. Solution: Provision an Azure Event Grid. Configure event filtering to evaluate the device identifier. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing an Azure Service application that processes queue data when it receives a message from a mobile application. Messages may not be sent to the service consistently. You have the following requirements: Queue size must not grow larger than 80 gigabytes (GB). Use first-in-first-out (FIFO) ordering of messages. Minimize Azure costs. You need to implement the messaging solution. Solution: Use the .Net API to add a message to an Azure Storage Queue from the mobile application. Create an Azure Function App that uses an Azure Storage Queue trigger. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing an Azure Service application that processes queue data when it receives a message from a mobile application. Messages may not be sent to the service consistently. You have the following requirements: Queue size must not grow larger than 80 gigabytes (GB). Use first-in-first-out (FIFO) ordering of messages. Minimize Azure costs. You need to implement the messaging solution. Solution: Use the .Net API to add a message to an Azure Storage Queue from the mobile application. Create an Azure VM that is triggered from Azure Storage Queue events. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a solution that will use Azure messaging services. You need to ensure that the solution uses a publish-subscribe model and eliminates the need for constant polling. What are two possible ways to achieve the goal?

- [x] Service Bus.
- [ ] Event Hub.
- [x] Event Grid.
- [ ] Queue.


### A company is implementing a publish-subscribe (Pub/Sub) messaging component by using Azure Service Bus. You are developing the first subscription application. In the Azure portal you see that messages are being sent to the subscription for each topic. You create and initialize a subscription client object by supplying the correct details, but the subscription application is still not consuming the messages. You need to ensure that the subscription client processes all messages. Which code segment should you use?

- [ ] await subscriptionClient.AddRuleAsync(new RuleDescription(RuleDescription.DefaultRuleName, new TrueFilter()));.
- [ ] subscriptionClient = new SubscriptionClient(ServiceBusConnectionString, TopicName, SubscriptionName);.
- [ ] await subscriptionClient.CloseAsync();.
- [x] subscriptionClient.RegisterMessageHandler(ProcessMessagesAsync, messageHandlerOptions);.


### You are developing an Azure solution to collect point-of-sale (POS) device data from 2,000 stores located throughout the world. A single device can produce 2 megabytes (MB) of data every 24 hours. Each store location has one to five devices that send data. You must store the device data in Azure Blob storage. Device data must be correlated based on a device identifier. Additional stores are expected to open in the future. You need to implement a solution to receive the device data. Solution: Provision an Azure Event Hub. Configure the machine identifier as the partition key and enable capture. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### A company is developing a solution that allows smart refrigerators to send temperature information to a central location. The solution must receive and store messages until they can be processed. You create an Azure Service Bus instance by providing a name, pricing tier, subscription, resource group, and location. You need to complete the configuration. Which Azure CLI or PowerShell command should you run?

- [ ] az group create --name fridge-rg --location fridge-loc.
- [ ] New-AzureRmServiceBusNamespace -ResourceGroupName fridge-rg -NamespaceName fridge-ns -Location fridge-loc.
- [x] New-AzureRmServiceBusQueue -ResourceGroupName fridge-rg -NamespaceName fridge-ns -Name fridge-q -EnablePartitioning $False.
- [ ] az servicebus namespace create --resource-group fridge-rg --name fridge-rg --location fridge-loc.


### Your company has an azure subscription that includes a storage account, a resource group, a blob container and a file share. A fellow administrator named Jon Ross used an Azure Resource Manager template to deploy a virtual machine and an Azure Storage account. You need to identify the Azure Resource Manager template the Jon Ross used. Solution: You access the Container blade. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### Your company has an azure subscription that includes a storage account, a resource group, a blob container and a file share. A fellow administrator named Jon Ross used an Azure Resource Manager template to deploy a virtual machine and an Azure Storage account. You need to identify the Azure Resource Manager template the Jon Ross used. Solution: You access the Virtual Machine blade. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### Your company has an azure subscription that includes a storage account, a resource group, a blob container and a file share. A fellow administrator named Jon Ross used an Azure Resource Manager template to deploy a virtual machine and an Azure Storage account. You need to identify the Azure Resource Manager template the Jon Ross used. Solution: You access the Resource Group blade. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing a web app named mywebapp1. Mywebapp1 uses the address myapp1.azurewebsites.net. You protect mywebapp1 by implementing an Azure Web Application Firewall (WAF). The traffic to mywebapp1 is routed through an Azure Application Gateway instance that is also used by other web apps. You want to secure all traffic to mywebapp1 by using SSL. Solution: You open the Azure Application Gateway's HTTP setting and set the Override backend path option to mywebapp1.azurewebsites.net. You then enable the Use for App service option. Does this meet the goal?

- [x] Yes.
- [ ] No.


### You are developing a web app named mywebapp1. Mywebapp1 uses the address myapp1.azurewebsites.net. You protect mywebapp1 by implementing an Azure Web Application Firewall (WAF). The traffic to mywebapp1 is routed through an Azure Application Gateway instance that is also used by other web apps. You want to secure all traffic to mywebapp1 by using SSL. Solution: You configure mywebapp1 to run in an Azure App service environment (ASE). Does this meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a web app named mywebapp1. Mywebapp1 uses the address myapp1.azurewebsites.net. You protect mywebapp1 by implementing an Azure Web Application Firewall (WAF). The traffic to mywebapp1 is routed through an Azure Application Gateway instance that is also used by other web apps. You want to secure all traffic to mywebapp1 by using SSL. Solution: You open the Azure Application Gateway's HTTP setting and set the Override backend path option to mywebapp1.azurewebsites.net. You then add an authentication certificate for mywebapp1.azurewebsites.net. Does this meet the goal?

- [ ] Yes.
- [x] No.


### Your company has a web app named WebApp1. You use the WebJobs SDK to design a triggered App Service background task that automatically invokes a function in the code every time new data is received in a queue. You are preparing to configure the service processes a queue data item. Which of the following is the service you should use?

- [ ] Logic Apps.
- [x] WebJobs.
- [ ] Flow.
- [ ] Functions.


### Your company has an Azure subscription. You need to deploy a number of Azure virtual machines to the subscription by using Azure Resource Manager (ARM) templates. The virtual machines will be included in a single availability set. You need to ensure that the ARM template allows for as many virtual machines as possible to remain accessible in the event of fabric failure or maintenance. Which of the following is the value that you should configure for the platformFaultDomainCount property?

- [ ] 10.
- [ ] 30.
- [ ] Min Value.
- [x] Max Value.


### You have two Hyper-V hosts named Host1 and Host2. Host1 has an Azure virtual machine named VM1 that was deployed by using a custom Azure Resource Manager template. You need to move VM1 to Host2. What should you do?

- [ ] From the Update management blade, click Enable.
- [ ] From the Overview blade, move VM1 to a different subscription.
- [x] From the Redeploy blade, click Redeploy.
- [ ] From the Profile blade, modify the usage location.


### Your company has an Azure Kubernetes Service (AKS) cluster that you manage from an Azure AD-joined device. The cluster is located in a resource group. Developers have created an application named MyApp. MyApp was packaged into a container image. You need to deploy the YAML manifest file for the application. Solution: You install the Azure CLI on the device and run the kubectl apply -f myapp.yaml command. Does this meet the goal?

- [x] Yes.
- [ ] No.


### Your company has an Azure Kubernetes Service (AKS) cluster that you manage from an Azure AD-joined device. The cluster is located in a resource group. Developers have created an application named MyApp. MyApp was packaged into a container image. You need to deploy the YAML manifest file for the application. Solution: You install the docker client on the device and run the docker run -it microsoft/azure-cli:0.10.17 command. Does this meet the goal?

- [ ] Yes.
- [x] No.


### Your company has an Azure subscription. You need to deploy a number of Azure virtual machines to the subscription by using Azure Resource Manager (ARM) templates. The virtual machines will be included in a single availability set. You need to ensure that the ARM template allows for as many virtual machines as possible to remain accessible in the event of fabric failure or maintenance. Which of the following is the value that you should configure for the platformUpdateDomainCount property?

- [ ] 10.
- [ ] 20.
- [ ] 30.
- [x] 40.


### You are designing an Azure WebJob that will run on the same instances as a web app. You want to make use of a suitable WebJob type. The webjob type should also allow for the option to restrict the WebJob to a single instance. Solution: You configure the use of the Triggered WebJob type. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are designing an Azure WebJob that will run on the same instances as a web app. You want to make use of a suitable WebJob type. The webjob type should also allow for the option to restrict the WebJob to a single instance. Solution: You configure the use of the Continuous WebJob type. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You company has an on-premises deployment of MongoDB, and an Azure Cosmos DB account that makes use of the MongoDB API. You need to devise a strategy to migrate MongoDB to the Azure Cosmos DB account. You include the [Data Management Gateway] tool in your migration strategy.

- [ ] No change required.
- [x] mongorestore.
- [ ] Azure Storage Explorer.
- [ ] AzCopy.


### You are developing an application that processes Azure Blob storage events. Your application has the following requirements: Process transaction logs asynchronously for changes that occur to the blobs and the blob metadata. Process changes in the order in which they occurred. Retain changes for compliance reasons. Solution: You use Azure Event Grid with a subscriber Azure Function app. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing an application that processes Azure Blob storage events. Your application has the following requirements: Process transaction logs asynchronously for changes that occur to the blobs and the blob metadata. Process changes in the order in which they occurred. Retain changes for compliance reasons. Solution: You use Azure Monitor HTTP Data Collector API. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a mobile app that uses an Azure SQL Database named Weyland. The database contains a table names Customers that has a field named email_address. You want to implement dynamic data masking to hide the data in the email_address field. Solution: You run the follows transact-SQL statement: ALTER TABLE [dbo].[Weyland].[Customers] ALTER COLUMN [email_address] ADD MASKED WITH (FUNCTION = 'email()') Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing a mobile app that uses an Azure SQL Database named Weyland. The database contains a table names Customers that has a field named email_address. You want to implement dynamic data masking to hide the data in the email_address field. Solution: You run the Set-AzSqlDatabaseDataMaskingPolicy -DatabaseName 'Weyland' Powershell cmdlet Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a mobile app that uses an Azure SQL Database named Weyland. The database contains a table names Customers that has a field named email_address. You want to implement dynamic data masking to hide the data in the email_address field. Solution: You run the Set-AzSqlDatabaseDataMaskingRule -DatabaseName 'Weyland' -SchemaName 'dbo' -TableName 'Customers' -ColumnName 'email_address' -MaskingFunction 'email' Powershell cmdlet Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing an e-Commerce Web App. You want to use Azure Key Vault to ensure that sign-ins to the e-Commerce Web App are secured by using Azure App Service authentication and Azure Active Directory (AAD). What should you do on the e-Commerce Web App?

- [ ] Run the az keyvault secret command.
- [ ] Enable Azure AD Connect.
- [x] Enable Managed Service Identity (MSI).
- [ ] Create an Azure AD service principal.


### You are developing a web app that uses Azure Active Directory (Azure AD) for authentication. You want to configure the web app to use multifactor authentication. What should you do?

- [ ] Enable mobile app authentication.
- [ ] In Azure AD conditional access, enable the baseline policy.
- [x] In Azure AD, create a conditional access policy.
- [ ] Install the Azure Multi-Factor Authentication Server.


### You are creating an Azure key vault using PowerShell. Objects deleted from the key vault must be kept for a set period of 90 days. Which two of the following parameters must be used in conjunction to meet the requirement? (Choose two.)

- [ ] EnabledForDeployment.
- [x] EnablePurgeProtection.
- [ ] EnabledForTemplateDeployment.
- [x] EnableSoftDelete.


### Your company has an Azure Active Directory (Azure AD) environment. Users occasionally connect to Azure AD via the Internet. You need to ensure that users who connect to Azure AD via the internet using an unidentified IP address, are automatically instructed to change their passwords. Solution: You configure the use of Azure Key Vault. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### Your company has an Azure Active Directory (Azure AD) environment. Users occasionally connect to Azure AD via the Internet. You need to ensure that users who connect to Azure AD via the internet using an unidentified IP address, are automatically instructed to change their passwords. Solution: You configure the use of Azure AD Identity Protection. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### Your company has an Azure Active Directory (Azure AD) environment. Users occasionally connect to Azure AD via the Internet. You need to ensure that users who connect to Azure AD via the internet using an unidentified IP address, are automatically instructed to change their passwords. Solution: You configure the use of Azure AD Privileged Identity Management. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You manage an Azure SQL database that allows for Azure AD authentication. You need to make sure that database developers can connect to the SQL database via Microsoft SQL Server Management Studio (SSMS). You also need to make sure the developers use their on-premises Active Directory account for authentication. Your strategy should allow for authentication prompts to be kept to a minimum. Which of the following should you implement?

- [ ] Azure AD token.
- [ ] Azure Multi-Factor authentication.
- [x] Active Directory integrated authentication.
- [ ] OATH software tokens.


### You are developing an application to transfer data between on-premises file servers and Azure Blob storage. The application stores keys, secrets, and certificates in Azure Key Vault and makes use of the Azure Key Vault APIs. You want to configure the application to allow recovery of an accidental deletion of the key vault or key vault objects for 90 days after deletion. What should you do?

- [ ] Run the Add-AzKeyVaultKey cmdlet.
- [x] Run the az keyvault update --enable-soft-delete true --enable-purge-protection true CLI.
- [ ] Implement virtual network service endpoints for Azure Key Vault.
- [ ] Run the az keyvault update --enable-soft-delete false CLI.


### You are configuring a web app that delivers streaming video to users. The application makes use of continuous integration and deployment. You need to ensure that the application is highly available and that the users' streaming experience is constant. You also want to configure the application to store data in a geographic location that is nearest to the user. Solution: You include the use of Azure Redis Cache in your design. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are configuring a web app that delivers streaming video to users. The application makes use of continuous integration and deployment. You need to ensure that the application is highly available and that the users' streaming experience is constant. You also want to configure the application to store data in a geographic location that is nearest to the user. Solution: You include the use of an Azure Content Delivery Network (CDN) in your design. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are configuring a web app that delivers streaming video to users. The application makes use of continuous integration and deployment. You need to ensure that the application is highly available and that the users' streaming experience is constant. You also want to configure the application to store data in a geographic location that is nearest to the user. Solution: You include the use of a Storage Area Network (SAN) in your design. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You develop a Web App on a tier D1 app service plan. You notice that page load times increase during periods of peak traffic. You want to implement automatic scaling when CPU load is above 80 percent. Your solution must minimize costs. What should you do first?

- [ ] Enable autoscaling on the Web App.
- [ ] Switch to the Premium App Service tier plan.
- [x] Switch to the Standard App Service tier plan.
- [ ] Switch to the Azure App Services consumption plan.


### You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance. Solution: You configure Basic gateway credentials for the Azure resource. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance. Solution: You configure Client cert gateway credentials for the HTTP(s) endpoint. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance. Solution: You configure Basic gateway credentials for the HTTP(s) endpoint. Does the solution meet the goal?

- [ ] Yes.
- [x] No.


### You are developing a solution for a public facing API. The API back end is hosted in an Azure App Service instance. You have implemented a RESTful service for the API back end. You must configure back-end authentication for the API Management service instance. Solution: You configure Client cert gateway credentials for the Azure resource. Does the solution meet the goal?

- [x] Yes.
- [ ] No.


### You are developing a .NET Core MVC application that allows customers to research independent holiday accommodation providers. You want to implement Azure Search to allow the application to search the index by using various criteria to locate documents related to accommodation venues. You want the application to list holiday accommodation venues that fall within a specific price range and are within a specified distance to an airport. What should you do?

- [ ] Configure the SearchMode property of the SearchParameters class.
- [ ] Configure the QueryType property of the SearchParameters class.
- [ ] Configure the Facets property of the SearchParameters class.
- [x] Configure the Filter property of the SearchParameters class.


### You are a developer at your company. You need to edit the workflows for an existing Logic App. What should you use?

- [ ] The Enterprise Integration Pack (EIP).
- [ ] The Logic App Code View.
- [ ] The API Connections.
- [x] The Logic Apps Designer.


### You are developing an application that applies a set of governance policies for internal and external services, as well as for applications. You develop a stateful ASP.NET Core 2.1 web application named PolicyApp and deploy it to an Azure App Service Web App. The PolicyApp reacts to events from Azure Event Grid and performs policy actions based on those events. You have the following requirements: Authentication events must be used to monitor users when they sign in and sign out. All authentication events must be processed by PolicyApp. Sign outs must be processed as fast as possible. What should you do?

- [ ] Create a new Azure Event Grid subscription for all authentication events. Use the subscription to process sign-out events.
- [ ] Create a separate Azure Event Grid handler for sign-in and sign-out events.
- [ ] Create separate Azure Event Grid topics and subscriptions for sign-in and sign-out events.
- [x] Add a subject prefix to sign-out events. Create an Azure Event Grid subscription. Configure the subscription to use the subjectBeginsWith filter.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to add code at line AM09 to ensure that users can review content using ContentAnalysisService. How should you complete the code?

![Question 193 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 193 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 193 part 3](images/question193.jpeg)

- [ ] Box 1: "oauth2Permissions": ["login"]. Box 2: oauth2AllowImplicitFlow: true.
- [x] Box 1: "oauth2AllowIdTokenImplicitFlow": true. Box 2: "oauth2AllowImplicitFlow": true.
- [ ] Box 1: "allowPublicClient": true. Box 2: "knownClientApplications": ["ContentAnalysisService"].
- [ ] Box 1: "oauth2Permissions": ["login"]. Box 2: "preAuthorizedApplications": ["SPA"].


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to add code at line AM10 of the application manifest to ensure that the requirement for manually reviewing content can be met. How should you complete the code?

![Question 194 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 194 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 194 part 3](images/question194.jpeg)

- [x] Box 1: sid. Box 2: email.
- [ ] Box 1: platf. Box 2: sid.
- [ ] Box 1: tenant_ctry. Box 2: upn.
- [ ] Box 1: sid. Box 2: enfpolids.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to ensure that network security policies are met. How should you configure network security?

![Question 195 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 195 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 195 part 3](images/question195.jpeg)

- [ ] SSL certificate: Self-signed certificate. Proxy type: nginx.
- [ ] SSL certificate: Self-signed certificate. Proxy type: Azure Application Gateway.
- [ ] SSL certificate: Valid root certificate. Proxy type: nginx.
- [x] SSL certificate: Valid root certificate. Proxy type: Azure Application Gateway.


### You are building a website to access project data related to teams within your organization. The website does not allow anonymous access. Authentication is performed using an Azure Active Directory (Azure AD) app named internal. The website has the following authentication requirements: Azure AD users must be able to login to the website. Personalization of the website must be based on membership in Active Directory groups. You need to configure the application's manifest to meet the authentication requirements. How should you configure the manifest?

![Question 196](images/question196.png)

- [ ] Box 1: "optionalClaims". Box 2: "allowPublicClient".
- [ ] Box 1: "optionalClaims". Box 2: "requiredResourceAccess".
- [ ] Box 1: "groupMembershipClaims". Box 2: "oauth2Permissions".
- [x] Box 1: "groupMembershipClaims". Box 2: "oauth2AllowimplicitFlow".


### You are developing an Azure solution. You need to develop code to access a secret stored in Azure Key Vault. How should you complete the code segment?

![Question 197](images/question197.png)

- [ ] Box 1: DefaultAzureCredential. Box 2: ClientSecretCredential.
- [ ] Box 1: CloudCltents. Box 2: ClientSecretCredential.
- [ ] Box 1: ClientSecretCredential. Box 2: SecretClient.
- [x] Box 1: SecretClient. Box 2: DefaultAzureCredential.


### You are developing a web application that makes calls to the Microsoft Graph API. You register the application in the Azure portal and upload a valid X509 certificate. You create an appsettings.json file containing the certificate name, client identifier for the application, and the tenant identifier of the Azure Active Directory (Azure AD). You create a method named ReadCertificate to return the X509 certificate by name. You need to implement code that acquires a token by using the certificate. How should you complete the code segment?

![Question 198](images/question198.jpg)

- [ ] Box 1: ConfidentialClientApplicationBuilder. Box 2: app.
- [x] Box 1: ConfidentialClientApplicationBuilder. Box 2: scopes.
- [ ] Box 1: GetAccountAsync(). Box 2: scopes.
- [ ] Box 1: ConfidentialClientApplication. Box 2: config.


### You are developing an ASP.NET Core Web API web service. The web service uses Azure Application Insights for all telemetry and dependency tracking. The web service reads and writes data to a database other than Microsoft SQL Server. You need to ensure that dependency tracking works for calls to the third-party database. Which two dependency telemetry properties should you use?

- [ ] Telemetry.Context.Cloud.RoleInstance.
- [x] Telemetry.Id.
- [ ] Telemetry.Name.
- [x] Telemetry.Context.Operation.Id.
- [ ] Telemetry.Context.Session.Id.


### You are developing an Azure App Service hosted ASP.NET Core web app to deliver video-on-demand streaming media. You enable an Azure Content Delivery Network (CDN) Standard for the web endpoint. Customer videos are downloaded from the web app by using the following example URL: http://www.contoso.com/content.mp4?quality=1. All media content must expire from the cache after one hour. Customer videos with varying quality must be delivered to the closest regional point of presence (POP) node. You need to configure Azure CDN caching rules. Which options should you use?

![Question 200](images/question200.jpeg)

- [x] Caching behavior: Override. Cache expiration duration: 1 hour. Query string caching behavior: Cache every unique URL.
- [ ] Caching behavior: Bypass cache. Cache expiration duration: 1 day. Query string caching behavior: Bypass caching for query strings.
- [ ] Caching behavior: Set if missing. Cache expiration duration: 1 second. Query string caching behavior: Ignore query strings.
- [ ] Caching behavior: Override. Cache expiration duration: 1 hour. Query string caching behavior: Ignore query strings.


### You develop a web app that uses tier D1 app service plan by using the Web Apps feature of Microsoft Azure App Service. Spikes in traffic have caused increases in page load times. You need to ensure that the web app automatically scales when CPU load is about 85 percent and minimize costs. Which four actions should you perform in sequence?

![Question 201](images/question201.jpg)

- [x] Box 1: Configure the web app to the Standard App Service tier. Box 2: Enable autoscaling on the web app. Box 3: Add a Scale rule. Box 4: Configure a Scale condition.
- [ ] Box 1: Enable autoscaling on the web app. Box 2: Add a Scale rule. Box 3:Configure a Scale condition. Box 4:Switch to an Azure App Services consumption plan.
- [ ] Box 1: Configure the web app to the Standard App Service tier. Box 2: Enable autoscaling on the web app. Box 3: Configure a Scale condition. Box 4: SecretClient.
- [ ] Box 1: Switch to an Azure App Services consumption plan. Box 2: Configure the web app to the Premium App Service tier. Box 3: Enable autoscaling on the web app. Box 4: Configure a Scale condition.


### A company backs up all manufacturing data to Azure Blob Storage. Admins move blobs from hot storage to archive tier storage every month. You must automatically move blobs to Archive tier after they have not been modified within 180 days. The path for any item that is not archived must be placed in an existing queue. This operation must be performed automatically once a month. You set the value of TierAgeInDays to -180. How should you configure the Logic App?

![Question 202](images/question202.jpeg)

- [ ] Box 1: Put a message on a queue. Box 2: Recurrence. Box 3: Condition. Box 4: When there are messages in a queue. Box 5: List blobs 2.
- [ ] Box 1: Recurrence. Box 2: Condition. Box 3: When there are messages in a queue. Box 4: Tier blob. Box 5: List blobs 2.
- [ ] Box 1: Recurrence. Box 2: Condition. Box 3: Put a message on a queue. Box 4: When there are messages in a queue. Box 5: Tier blob.
- [x] Box 1: Recurrence. Box 2: Condition. Box 3: Put a message on a queue. Box 4: Tier blob. Box 5: List blobs 2.


### You have an Azure Web app that uses Cosmos DB as a data store. You create a CosmosDB container by running the following PowerShell script: $resourceGroupName = 'testResourceGroup' $accountName = 'testCosmosAccount' $databaseName = 'testDatabase' $containerName = 'testContainer' $partitionKeyPath = '/EmployeeId' $autoscaleMaxThroughput = 5000 New-AzCosmosDBSqlContainer - -ResourceGroupName $resourceGroupName -AccountName $accountName -DatabaseName $databaseName -Name $containerName -PartitionKeyKind Hash -PartitionKeyPath $partitionKeyPath -AutoscaleMaxThroughput $autoscaleMaxThroughput You create the following queries that target the container: SELECT * FROM c WHERE c.EmployeeId > '12345' SELECT * FROM c WHERE c.UserID = '12345'. Question 1: The minimum throughput for the container is 400 R/Us.

- [ ] Yes.
- [x] No.


### You have an Azure Web app that uses Cosmos DB as a data store. You create a CosmosDB container by running the following PowerShell script: $resourceGroupName = 'testResourceGroup' $accountName = 'testCosmosAccount' $databaseName = 'testDatabase' $containerName = 'testContainer' $partitionKeyPath = '/EmployeeId' $autoscaleMaxThroughput = 5000 New-AzCosmosDBSqlContainer - -ResourceGroupName $resourceGroupName -AccountName $accountName -DatabaseName $databaseName -Name $containerName -PartitionKeyKind Hash -PartitionKeyPath $partitionKeyPath -AutoscaleMaxThroughput $autoscaleMaxThroughput You create the following queries that target the container: SELECT * FROM c WHERE c.EmployeeId > '12345' SELECT * FROM c WHERE c.UserID = '12345'. Question 2: The first query statement is an in-partition query.

- [ ] Yes.
- [x] No.


### You have an Azure Web app that uses Cosmos DB as a data store. You create a CosmosDB container by running the following PowerShell script: $resourceGroupName = 'testResourceGroup' $accountName = 'testCosmosAccount' $databaseName = 'testDatabase' $containerName = 'testContainer' $partitionKeyPath = '/EmployeeId' $autoscaleMaxThroughput = 5000 New-AzCosmosDBSqlContainer - -ResourceGroupName $resourceGroupName -AccountName $accountName -DatabaseName $databaseName -Name $containerName -PartitionKeyKind Hash -PartitionKeyPath $partitionKeyPath -AutoscaleMaxThroughput $autoscaleMaxThroughput You create the following queries that target the container: SELECT * FROM c WHERE c.EmployeeId > '12345' SELECT * FROM c WHERE c.UserID = '12345'. Question 3: The second query statement is a cross-partition query.

- [x] Yes.
- [ ] No.


### Your Azure Active Directory Azure (Azure AD) tenant has an Azure subscription linked to it. Your developer has created a mobile application that obtains Azure AD access tokens using the OAuth 2 implicit grant type. The mobile application must be registered in Azure AD. You require [a redirect URI] from the developer for registration purposes.

- [x] No change required.
- [ ] a secret.
- [ ] a login hint.
- [ ] a client ID.


### You develop an ASP.NET Core MVC application. You configure the application to track webpages and custom events. You need to identify trends in application usage. Which Azure Application Insights Usage Analysis features should you use?

![Question 207](images/question207.png)

- [x] Box 1: Funnels. Box 2: Impact. Box 3: Retention. Box 4: User Flows.
- [ ] Box 1: Impact. Box 2: Funnels. Box 3: Retention. Box 4: User Flows.
- [ ] Box 1: Users. Box 2: Impact. Box 3: Retention. Box 4: User Flows.
- [ ] Box 1: Impact. Box 2: Users. Box 3: User Flows. Box 4: Funnels.


### You are developing an application that uses a premium block blob storage account. You are optimizing costs by automating Azure Blob Storage access tiers. You apply the following policy rules to the storage account. You must determine the implications of applying the rules to the data. (Line numbers are included for reference only.) Question 1: Block blobs prefixed with container1/salesorders or container2/inventory which have not been modified in over 60 days are moved to cool storage. Blobs that have not been modified in 120 days are moved to the archive tier.

![Question 208](images/question208_209_210_211.png)

- [x] Yes.
- [ ] No.


### You are developing an application that uses a premium block blob storage account. You are optimizing costs by automating Azure Blob Storage access tiers. You apply the following policy rules to the storage account. You must determine the implications of applying the rules to the data. (Line numbers are included for reference only.) Question 2: Blobs are moved to cool storage if they have not been accessed for 30 days.

![Question 209](images/question208_209_210_211.png)

- [x] Yes.
- [ ] No.


### You are developing an application that uses a premium block blob storage account. You are optimizing costs by automating Azure Blob Storage access tiers. You apply the following policy rules to the storage account. You must determine the implications of applying the rules to the data. (Line numbers are included for reference only.) Question 3: Blobs will automatically be tiered from cool back to hot if accessed again after being tiered to cool.

![Question 210](images/question208_209_210_211.png)

- [x] Yes.
- [ ] No.


### You are developing an application that uses a premium block blob storage account. You are optimizing costs by automating Azure Blob Storage access tiers. You apply the following policy rules to the storage account. You must determine the implications of applying the rules to the data. (Line numbers are included for reference only.) Question 4: All block blobs older than 730 days will be deleted.

![Question 211](images/question208_209_210_211.png)

- [ ] Yes.
- [x] No.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to store the user agreements. Where should you store the agreement after it is completed?

![Question 212 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 212 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)

- [ ] Azure Storage queue.
- [x] Azure Event Hub.
- [ ] Azure Service Bus topic.
- [ ] Azure Event Grid topic.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to monitor ContentUploadService according to the requirements. Which command should you use?

![Question 213 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 213 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)

- [ ] az monitor metrics alert create Cn alert Cg … - -scopes … - -condition "avg Percentage CPU > 8".
- [ ] az monitor metrics alert create Cn alert Cg … - -scopes … - -condition "avg Percentage CPU > 800".
- [x] az monitor metrics alert create Cn alert Cg … - -scopes … - -condition "CPU Usage > 800".
- [ ] az monitor metrics alert create Cn alert Cg … - -scopes … - -condition "CPU Usage > 8".


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to investigate the http server log output to resolve the issue with the ContentUploadService. Which command should you use first?

![Question 214 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 214 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)

- [ ] az webapp log.
- [ ] az ams live-output.
- [ ] az monitor activity-log.
- [x] az container attach.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to implement the bindings for the CheckUserContent function. How should you complete the code segment?

![Question 215 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 215 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 215 part 3](images/question215.jpeg)

- [ ] Box 1: [CosmosDBTrigger("content", "userContent")]. Box 2: [Table("content", "userContent", "{name}")].
- [ ] Box 1: [CosmosDBTrigger("content", "userContent")]. Box 2: [Queue("userContent")].
- [ ] Box 1: [BlobTrigger("userContent/{name}")]. Box 2: [Blob("userContent/{name}", FileAccess.Write)].
- [x] Box 1: [QueueTrigger("userContent")]. Box 2: [Blob("userContent/{name}", FileAccess.Write)].


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to add markup at line AM04 to implement the ContentReview role. How should you complete the markup?

![Question 216 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 216 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 216 part 3](images/question216.jpeg)

- [ ] Box 1: allowedAccountTypes. Box 2: User. Box 3: value.
- [ ] Box 1: role. Box 2: User. Box 3: value.
- [x] Box 1: allowedMemberTypes. Box 2: User. Box 3: value.
- [ ] Box 1: allowedMemberTypes. Box 2: value. Box 3: User.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to add YAML markup at line CS17 to ensure that the ContentUploadService can access Azure Storage access keys. How should you complete the YAML markup?

![Question 217 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 217 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 217 part 3](images/question217.jpeg)

- [ ] Box 1: volumes. Box 2: volumeMounts. Box 3: secret.
- [x] Box 1: volumeMounts. Box 2: volumes. Box 3: secret.
- [ ] Box 1: envVar. Box 2: secretValues. Box 3: environmentVariables.
- [ ] Box 1: secret. Box 2: environmentVariables. Box 3: secretValues.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to deploy the CheckUserContent Azure Function. The solution must meet the security and cost requirements. Which hosting model should you use?

![Question 218 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 218 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)

- [ ] Premium plan.
- [x] App Service plan.
- [ ] Consumption plan.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to ensure that validation testing is triggered per the requirements. How should you complete the code segment?

![Question 219 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 219 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)
![Question 219 part 3](images/question219.jpeg)

- [x] Box 1: ImagePushed. Box 2: repository. Box 3: topic.
- [ ] Box 1: ImageDeployed. Box 2: service. Box 3: imageCollection.
- [ ] Box 1: RepositoryUpdated. Box 2: service. Box 3: imageCollection.
- [ ] Box 1: RepositoryItem. Box 2: aci. Box 3: topic.


### You are a developer for Contoso, Ltd. The company has a social networking website that is developed as a Single Page Application (SPA). The main web application for the social networking website loads user uploaded content from blob storage. You are developing a solution to monitor uploaded data for inappropriate content. The following process occurs when users upload content by using the SPA: Messages are sent to ContentUploadService. Content is processed by ContentAnalysisService. After processing is complete, the content is posted to the social network or a rejection message is posted in its place. The ContentAnalysisService is deployed with Azure Container Instances from a private Azure Container Registry named contosoimages. The solution will use eight CPU cores. Azure Active Directory: Contoso, Ltd. uses Azure Active Directory (Azure AD) for both internal and guest accounts. Requirements: ContentAnalysisService - The company's data science group built ContentAnalysisService which accepts user generated content as a string and returns a probable value for inappropriate content. Any values over a specific threshold must be reviewed by an employee of Contoso, Ltd. You must create an Azure Function named CheckUserContent to perform the content checks. Costs: You must minimize costs for all Azure services. Manual review: To review content, the user must authenticate to the website portion of the ContentAnalysisService using their Azure AD credentials. The website is built using React and all pages and API endpoints require authentication. In order to review content a user must be part of a ContentReviewer role. All completed reviews must include the reviewer's email address for auditing purposes. High availability: All services must run in multiple regions. The failure of any service in a region must not impact overall application availability. Monitoring: An alert must be raised if the ContentUploadService uses more than 80 percent of available CPU cores. Security: You have the following security requirements: Any web service accessible over the Internet must be protected from cross site scripting attacks. All websites and services must use SSL from a valid root certificate authority. Azure Storage access keys must only be stored in memory and must be available only to the service. All Internal services must only be accessible from internal Virtual Networks (VNets). All parts of the system must support inbound and outbound traffic restrictions. All service calls must be authenticated by using Azure AD. User agreements: When a user submits content, they must agree to a user agreement. The agreement allows employees of Contoso, Ltd. to review content, store cookies on user devices, and track user's IP addresses. Information regarding agreements is used by multiple divisions within Contoso, Ltd. User responses must not be lost and must be available to all parties regardless of individual service uptime. The volume of agreements is expected to be in the millions per hour. Validation testing: When a new version of the ContentAnalysisService is available the previous seven days of content must be processed with the new version to verify that the new version does not significantly deviate from the old version. Issues: Users of the ContentUploadService report that they occasionally see HTTP 502 responses on specific pages. Code - ContentUploadService - ApplicationManifest. You need to configure the ContentUploadService deployment. Which two actions should you perform?

![Question 220 part 1](images/question193_194_195_212_213_214_215_216_217_218_219_220_1.jpeg)
![Question 220 part 2](images/question193_194_195_212_213_214_215_216_217_218_219_220_2.jpeg)

- [x] Add the following markup to line CS23: type: Private.
- [ ] Add the following markup to line CS24: osType: Windows.
- [x] Add the following markup to line CS24: osType: Linux.
- [ ] Add the following markup to line CS23: type: Public.

