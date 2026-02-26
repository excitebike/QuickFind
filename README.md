# QuickFind
Sidecar navigation to quickly access the details page of a record simply by
typing the record’s key value into one of the multiple input options available.


![quickfind](https://github.com/user-attachments/assets/1c1324fb-643b-4223-89da-4029a623fffd)

Full demo video can be found in the attachments to this repo.  

# Goals
## Main Goal
Reduce the query cost and user wait time of reading multiple records upon opening a list page
form only to have a user filter to find a specific record. 

## Secondary goals
1) Reduce the number of clicks and total active user interaction time to navigate to a details form
page.

2) Group frequently searched forms into one central workspace to help streamline a user’s
experience.

All small things, but compounded across an organization, we would hopefully see an improvement in
application performance and the user experience resulting in increased customer satisfaction.

# Design tenants
1) No further technical development required.

   o Allow configurations and setups to dynamically drive how the form can be utilized within each organization as well as with each user.


2) No security configuration required.
   
      o The main quick find forms have been added to the common main menu and their
       security duties have been added to the SysUser role.
    
      o All the Admin setup forms have been added to new duties.

3) Minimal user setup.
   
  	 o Although there are a few options each user can configure if they choose, quick find is
  	 ready to go once the initial organizational setup is complete.

4) Clean and intuitive form design and user interaction.

# Logic 

Each organization defines what menu items are available by populating a new setup table.  For most system menu items, logic will auto populate the necessary meta data fields, but the fields can also be manually set.  

<img width="708" height="333" alt="image" src="https://github.com/user-attachments/assets/8b0b07f3-7c87-4f06-a07d-47041606f76a" />


Main execution logic. 
<img width="1016" height="1173" alt="image" src="https://github.com/user-attachments/assets/f2710fe3-6983-4cdc-89aa-ee1ec57f162d" />

