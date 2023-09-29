# Creating-Administrative-Users

<p align="center">

</p>

<h1>Active Directory - Creating Administrative Users</h1>
This tutorial outlines the creation of administrative users in Active Directory using virtual machines in Microsoft Azure.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Client-1 virtual machine
- DC-1 virtual machine

*Using remote desktop connect to the client-1 virtual machine*
*Using remote desktop log onto the DC-1 virtual machine using the fully qualified domain name*
  
 ![Logging Into DC-1 With New Credentials](https://github.com/Ken7281/Creating-Administrative-Users/assets/142465932/32ec9bb0-9fea-443b-a374-dfc87063f218)

 *On the DC-1 virtual machine, open Active Directory Users & Computers*
 *Right click on mydomain.com select new and then select organizational units* 

 ![Creating Organizational Units](https://github.com/Ken7281/Creating-Administrative-Users/assets/142465932/6b72251a-872a-4316-88c0-9314852a0b2b)

 *Create two organizational units under mydomain.com*

 *Click on one of the newly created organizational unit and right click it.*
 *Select new and select user*
 *Create a name and password for the user*

 ![Creating a name for the new user](https://github.com/Ken7281/Creating-Administrative-Users/assets/142465932/2b666e21-b2e1-4a90-ad31-f3116ad56929)

  *Right click on the newly created user and select properties*

  ![Changing The Properties of the user](https://github.com/Ken7281/Creating-Administrative-Users/assets/142465932/56c24960-2511-47e6-a88d-6a7cd677b225)
  
*Under properties Select the member of tab and select add*
  ![Changing the member group of the user](https://github.com/Ken7281/Creating-Administrative-Users/assets/142465932/08c73e63-ceb7-4dae-a3da-a18c1b636084)

  *Type domain and select the check names box* 
  *Double click on the domain admins group select ok then apply and ok again to add the changes to the user group*

  *Log off of the DC-1 virtual machine and connect back to it using the newly created user*

  ![Logging onto DC-1 as the new user](https://github.com/Ken7281/Creating-Administrative-Users/assets/142465932/0b45eff1-9fb0-46be-ae27-420dc93b387d)

*The administrative user is now successfully created in active directory*
