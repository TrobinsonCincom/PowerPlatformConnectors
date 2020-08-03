## CPQSync

CPQSync Connector provides access to keep Master Data in sync with CPQSync and enteprise systems. 

## Pre-requisites
You will need the following to proceed:
* Access to your CPQSync  [Administration](https://www.cincomcpq.com/) area to access your API Key and Tenant Id

## Supported Operations
The connector supports the following operations:
* `Add Product`: Add a product to the catalog
* `Update Products`: Update a product in the catalog
* `GetProductCreatedSchema`: Get the schema to create a product
* `GetProductUpdatedSchema`: Get the schema to update a product
* `Product Created`: Trigger when Product is created
* `Product Updated`: Trigger when Product is updated

## Using the CPQSync Connector to Add a Product From Dynamics 365 to CPQSync
1. Navigate to [Power Automate](https://us.flow.com)
1. Create a flow using the "When a record is created" trigger from the Common Data Services connector
1. Create a connection for the trigger and select your environment
1. Select Products from the "Entity Name" dropdown  
1. Click "+ New Step" and select the "Add Product" action from the CPQSync connector
1. Navigate to [CCA](https://cca.cincomcpq.com) and copy your tenant Id and API key
1. Create a connection to the CPQSync connector by entering a connection name and typing "API [your-api-key]" in the API key field. Where [your-api-key] is the API key you copied from [CCA](https://cca.cincomcpq.com]
1. Map all fields from Dynamics 365 to CPQSync and click save
