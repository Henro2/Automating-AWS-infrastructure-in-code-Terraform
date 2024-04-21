## Automating AWS infrastructure in code (Terraform)

![alt text](images/Untitled.png)


I created **main.tf**  file in my PBL folder to store my terraform code.

   I coppied and pasted the the AWS provider resouce code and changed the region to US-EAST-1

   I also copied the VPC creation resouces and pasted 

   ![alt text](<images/Screenshot from 2024-04-12 09-22-10.png>)


   ## Subnets resource section

   I also inserted the aws resouce code for creating subnets in my new VPC. Note, I changed the available zone of pblic1 subnet to US-east-1a and Public2 to Us-east-1b. SO we have two avaiblabilty zones. A and B.

   ![alt text](<images/Screenshot from 2024-04-12 09-31-40.png>)

-  I ran terrafom apply and the VPC and the subnets where created sussessfully as shown below
SS
![alt text](<images/Unsaved Image 2.png>)


## Fixing The Problems By Code Refactoring

- Now i have to destroy my corrent infastructure so i can refactor my codes 

![alt text](images/destroy.png)

**Fixing Hard Coded Values**: We will introduce variables, and remove hard coding.

SO i have to edit     **main.tf** file 

