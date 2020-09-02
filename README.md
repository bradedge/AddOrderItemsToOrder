# Add_Order_Items_to_Order

__Designer__: Brad Edgerly
__Design Date__: 2020-08-31

__Purpose__: 
A professional services company users orders and order items to provide and fulfill commitments to its customers. 

The "Add Order Items to Order" Visualforce page increases the speed and accuracy of a sales representative creating a new order.

This Visualforce page allows sales representatives to quickly search for previous order items, select/deselect items, and save new order items against the originating order.

__Request__:
Please build out the Visualforce page ("force-app\main\default\pages\Add_Order_Items_to_Order") and required controllers.

You will find the mockup and requirements in /design/UserInterfaceMockup.png.  

You will find the entity relationship diagram in /design/EntityRelationshipDiagram.png.  

If you have questions, your team is here to help! Please contact brad.edgerly@creativesparq.ca who will point you in the right direction.  

# Prerequisits

1. Install Visual Studio Code  
2. Install Salesforce Extension Pack  
3. Log into dev hub  
4. Install Git  
5. Install Node.js and npm  

# Setup 
1. Navigate to your home directory in Visual Studio Code.  
2. Pull down repository.  
`git clone https://github.com/bradedge/AddOrderItemsToOrder.git`  
3. Navigate to project directory.  
`cd AddOrderItemsToOrder`  
4. Create a branch.  
`git branch mybranch`  
5. Check out branch.  
`git checkout mybranch`  
6. Open Visual Studio Code > File > Open Folder > AddOrderItemsToOrder  
7. Create scratch org.  
`sfdx force:org:create -s -f config/project-scratch-def.json -a MyScratch -d 30`  
8. Push repository into scratch org.  
`sfdx force:source:deploy -u MyScratch -x package.xml`  
9. Assign permission set to access fields  
`sfdx force:user:permset:assign --permsetname Order_And_Order_Item_Access --targetusername MyScratch`  
10. Populate data  
`sfdx force:data:tree:import -f assets/data/Order__c-Order_Item__c.json -u MyScratch`  
11. Happy coding!  

# Submit

1. Create admin user account:  
- User name: intake@creativesparq.ca.[your last name]
- Email address: intake@creativesparq.ca
2. Notify brad.edgerly@creativesparq.ca