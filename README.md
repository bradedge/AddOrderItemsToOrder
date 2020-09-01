# Add_Order_Items_to_Order

__Designer__: Brad Edgerly
__Design Date__: 2020-08-31

__Purpose__: 
A professional services company users orders and order items to provide and fulfill commitments to its customers. 

The "Add Order Items to Order" Visualforce page increases the speed and accuracy of a sales representative creating a new order.

This Visualforce page allows sales representatives to quickly search for previous order items, select/deselect items, and save new order items against the originating order.

__Request__:
Please create "force-app\main\default\pages\Add_Order_Items_to_Order" and required controllers.

# Setup 
1. Navigate to your home directory.
2. Pull down repository.
`git clone https://github.com/bradedge/AddOrderItemsToOrder.git`
3. Navidate to project directory.
`cd AddOrderItemsToOrder`
4. Create a branch and check it out.
`git branch mybranch`
`git checkout mybranch`
5. Open Visual Studio Code > File > Open Folder > AddOrderItemsToOrder
6. Create scratch org.
`sfdx force:org:create -s -f config/project-scratch-def.json -a MyScratch -d 30`
7. Push repository into scratch org.
`sfdx force:source:deploy -u MyScratch -x package.xml`
8. Assign permission set to access fields
`sfdx force:user:permset:assign --permsetname Order_And_Order_Item_Access --targetusername MyScratch`
9. Happy coding!

# Push back

1. Add changed files to staging.
`git add .`
2. Create snapshot.
`git commit -m “My commit”`
3. Send changes to remote repository.
`git push -u origin mybranch`
4. Notify Creative SparQ.