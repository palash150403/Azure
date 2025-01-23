# AZ-104 Notes

## Virtual Machines

#### Resource Group
-   It is a logic grouping of resources.

#### VM Architecture

![alt text](image-50.png)

-   When VM is cerated :-
    -   VM
    -   OS Disk (127 GiB)
    -   Network Interface
    -   Public IP
    -   Network security Group
    -   Virtual Network (VNet)

    are created along with VM.

-   AZ allows to scale the size of existing virtual machine.

#### OS Disk
-   You can attach new OS Disk or a Driver Disk to your VM. This will we added as a additional storage driver.

-   If you deallocate your VM then the data stored in tmp stored will also be removed. But if the data is stored in a extenally attached drive then data will persist.

-   You can take snapshot of OS Disk and then, You can create a new OS Disk based on that snapshot and then you can attach that newly created OS Disk to another VM.

-   We can deattach the existing OS disk of a VM and can attach it to another VM.

#### Disk Encryption Set
-   It is used to create your own encryption key and use that key to encrypt your Disk.
This encryption key is stored in KeyVault.

#### Custom script extension
-   Used to execute prewritten scripts that are executed when VM starts.

-   Steps:-
    -   First create a Storage account.
    -   Then create a container in it.
    -   Then upload your script over there.
    -   Now, while creating your VM in Advanced section Install extensiion over there configure your script.

#### Cloud Init
-   It also same as custome script, but here the script is pasted in advanced section while the creation proccess of VM.



## DNS for VM's

-   Create a VM
-   go into it's ip section

![alt text](image-16.png)

-   and save

![alt text](image-17.png)

## Storage Account

### Cretaing Blob Storage

![alt text](image-18.png)

### Uploading files on Blob Storage

-   Create Container

![alt text](image-19.png)

-   Upload files

![alt text](image-20.png)

### Give public access

![alt text](image-21.png)

![alt text](image-22.png)

![alt text](image-23.png)

### Access policy

-   Creating Access Policy

-   We use Access policy because once the tokens are generated then its permisssions cannot be chaged but. permission of policy can be changed so we create shared access tokens using policy, so we can change policy and that will change token's permission

![alt text](image-24.png)

-   Creating accesss tokens

![alt text](image-25.png)

### Change Access tiers

![alt text](image-26.png)

### Create Lifecycle Rule


![alt text](image-28.png)

![alt text](image-27.png)

![alt text](image-29.png)

![alt text](image-30.png)

#### Note:-

-   If there is a condition in which 2 rules and made. 
-   one rule says that if object is not acceed in last 14 days, then delete it.
-   and other rule states that if it is not accesed in 14 days then move to cool tier.
-   here a conflict is created so, the cheapest option over here will be taken into the considiration


### Creating Replication copies

-   need to enable blob versoning and blob change feed.

![alt text](image-31.png)

![alt text](image-32.png)

-   Replication copy is made

![alt text](image-33.png)


### Create snapshot

![alt text](image-34.png)

-   created snapshot

![alt text](image-35.png)

-   Do promote to apply changes of that snapshot

![alt text](image-36.png)

### Creating file share

![alt text](image-37.png)

![alt text](image-38.png)

-   Now to access files on your system

-   First click on connect 

![alt text](image-39.png)

-   now paste the script on your machine to view files.

![alt text](image-40.png)

### Allowing only acces from Vnet users

-   First create service endpoint

![alt text](image-41.png)

-   now go to storage account section

![alt text](image-42.png)

-   Configure and add Vnet

![alt text](image-43.png)

#### Creating Private Vnet Endpoint

![alt text](image-44.png)

![alt text](image-45.png)



## RBAC and Account Mangment

### How to cerate a user

-   first go to microsoft Enfra ID

![alt text](image-46.png)

-   then create a user

![alt text](image-47.png)

-   Whilw creating you can assign roles or grouops

![alt text](image-48.png)

-   user successfully created 

![alt text](image-49.png)
