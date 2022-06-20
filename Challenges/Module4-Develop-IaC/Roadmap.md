# Module 4 - Developing Infrastructure as Code for Deploying Environments

## Background
Fabrikam has decided to move forward with widescale deployment of their new cloud environment, but wants an easier way to manage and control deployments using infrastructure as code. While there has been progress completed in modernizing the components and improving the overall developer worklow, there are benefits of going to the cloud that will never be realized in its current state. The client has worked with Insight and trusts you as a developer to find the right way to implement this new requirement. The following is the outline of what Fabrikam wants in order to facilitate their IaC requirements..
   

Here is an overview of the design requirements for this build:
### Landing Zone Foundational Requirements
  * Log Analytics Workspace
  * Key Vault
  * Virtual Network
  * Storage Account
  * Tagging Standards on Azure Resources: ex. Cost Center, Environment, DeploymentType, Application Name
  * Deploy services with a Service Principal
  * Resource Group Organization Strategy
  * Use Terraform to build your landing zones - use modules as described in the Cloud Adoption Framework
  * Store Terraform State in Azure Storage
  * Proof of concept should be in 1 subscription and have a dev and test environment
### Architecture Deployment Requirements
  * Primary and Secondary Regions should be used. i.e. East US / West US or East US 2/Central US
  * Resource Group Organization: Each environment should have a resource group per region
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
  * Use of Terraform Cloud is optional but should be justified

### Documentation Requirements
  * Use Lucidcharts or Visio to create your diagrams
  * Leverage an Insight-branded powerpoint template for your presentation


# Deliverables
  * Documentation
    * A diagram depicting the application architecture that you have built in Azure, including the Landing Zone components
    * Create a flowchart depicting the infrastructure as code deployment process of creating the dev and test environment
  * Presentations
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
  * Sample code should be used where applicable to demonstrate a given service is configured properly
  * In each module, you may list out questions you have and schedule technical stakeholder meetings







