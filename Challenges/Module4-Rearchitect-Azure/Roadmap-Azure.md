# Module 4 - Re-Architecting the Application in Azure

## Background
Fabrikam has decided to rewrite this application and host it in a new architecture and set of environments in Azure. While there has been progress completed in modernizing the components and improving the overall developer worklow, there are benefits of going to the cloud that will never be realized in its current state. The client has worked with Insight in a series of design workshops. The following is the outline of the Highly available multi-region web application architecture that will the starting point for the new build of the application.
   ![](/Assets/multi-region-web-app-diagram.png)
   *Highly-Available Multi-Region Web Application in Azure*

Here is an overview of the design requirements for this build
### Landing Zone Foundational Requirements
  * Log Analytics Workspace
  * Key Vault
  * Virtual Network
  * Storage Account
  * Tagging Standards on Azure Resources: Cost Center, Environment, DeploymentType, Application Name
  * Deploy servics with a Service Principal
  * Resource Group Organization Strategy
  * Use Terraform to build your landing zones - use modules as described in the Cloud Adoption Framework
  * Store Terraform State in Azure Storage
  * Proof of concept should be in 1 subscription and have a dev and test environment
### Architecture Deployment Requirements
  * Primary and Secondary Regions should be used. i.e. East US / West US or East US 2/Central US
  * Ensure your solution is setup as active/passive with hot standby, using Front Door for failover
  * Resource Group Organization: Each environment should have a resource group per region
  * Each service should have a sample application or way of showing the resources is deployed
### Application Requirements
  * Application must have a web and api layers in a Azure App Service Plan
  * A function app should be created and deployed
### Data Requirements
  * An Azure SQL Database setup with geo-redundancy
  * A Cosmos DB is part of the application

### Other components
  * Azure Search should be configured
  * Demonstrate connection to each service

### DevOps Design Requirements
  * Host your source code in Github or Azure Repos
  * Create at least 1 working CI/CD pipeline in Azure Pipelines for the deployment of the web, api, or other application component.
  * Use Terraform and Azure Bicep throughout this solution

### Documentation Requirements
  * Use Lucidcharts or Visio to create your diagrams
  * Leverage an Insight-branded powerpoint template for your presentation


# Deliverables
  * Documentation
    * A diagram depicting the application architecture that you have built in Azure, including the Landing Zone components
    * Create a flowchart depicting the infrastructure as code deployment process of creating the dev and test environment
    * Create a flowchart depicting the flow of code from a developer to the web application
  * Build Artifacts
    * Present a brief overview of how the application components work together
    * Host your source code in Azure Repos
    * Demonstrate a working solution for each of the services that were deployed
  * Presentations
    * Progress Report Presentation # 1 and # 2 as specificed in the SOW
    * Closeout Presentation
      * Agenda
      * Summarize Modules 1-3: what problems were solved and what work you completed
      * Module 4
        * Summary of the current state architecture
        * Review of architecture diagrams and flows
        * Demo your as built solution in Azure
        * Demo your IaC deployment process for key services in the Architecture
        * Review the obstacles and challenges you encountered throughout the project
        * Since this is a proof of concept, what is the next phase?
          * Outline a list of enhancements, new features, and suggestions for the next phase


## Rules and References
  * Sample code should be used where applicable to demonstrate a givne service is configured properly
  * In each module, you may list out questions you have and schedule technical stakeholder meetings







