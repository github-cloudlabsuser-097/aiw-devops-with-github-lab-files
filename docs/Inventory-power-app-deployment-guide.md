**Setup Instructions for Power Platform App- Inventory Management System**
--------------------------------------------------------------------------
This deployment guide is designed to deploy a Power app into your Power platform environment. Inventory Management App can be used for updating the product details in a fully automated way. This app created by using workflows and Adaptive card.

**Pre-Requisite**

  1.	Azure Portal
      Login into Azure Portal and go to Azure Active directory.
      Add a user having licenses of Power apps, Power automate and Microsoft Teams Exploratory.

  2.  Power platform environment
      Login into power platform environment with your trial or organization account by clicking on the below link:
      https://powerapps.microsoft.com/en-us/ 
  
  3.  Add a business user in sharepoint list. For user details refer cloudlabs instructions.
  
      **Note: This user is going authenticate the Inventory Management Application.** 
  
  4. A sharepoint list to be created named Update Product details.
  
      **Note: This list will store the details of the Product update, the business entered through the inventory app.**
  
  5. Create an Azure SQL database connection string in the dataverse section of the power platform environment and validate it.
      
**Deployment**

  1. After login into the Power platform environment go to Power platform admin center and click on Apps and then click on Import Canvas App.
  2. After clicking on Import Canvas App, you will reach into import package details pane and validate the connection strings. While importing the application user need to validate the workflow as created new and connection string with Azure SQL database as update. Then click on the import button.
  3. It will take 5-10 minutes to complete the import operation and once it completed user can access the Inventory Management System App.
  4. CLick on the App to execute it, enter the business user credentials on it and go to update product screen and do an update of the price of any product. 
    
    
**Common errors**
  
  1. Authentication failed
  2. Connection string not listed
    
**to resolve the above errors you can choose following options**    
    
  1. Check the user connection string is available.
    
  2. If the Azure SQL database connection string not validated please create a connection string in dataverse section of the power platform.
