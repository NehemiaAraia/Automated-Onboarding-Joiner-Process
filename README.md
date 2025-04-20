# Automated Onboarding Joiner Process

Designed and deployed an automated employee onboarding flow using Power Automate, Entra ID, and Microsoft Forms. The system captures new hire information through form submissions, triggers a flow in Power Automate to create user accounts in Entra ID, and dynamically assigns users to the appropriate department security group based on their selected responses. This improved onboarding speed and ensured new users had the right access in place before their first day.

Tools & Resources
- **Microsoft Power Automate**: Used to design and run the automated workflows.
- **Microsoft Entra ID (Azure AD)**: Used to create user accounts and assign them to appropriate security groups.
- **Microsft Forms**: Used to collect data from new hires during onboarding process.



## Step by Step Process

1. Designed a form to collect essential employee information: Full Name, Email, Department, Start Date, etc.
   
   ![image](https://github.com/user-attachments/assets/bcdd1745-ad30-4dcd-9d35-a34012e16072)



2. Created a security group (IT) in Microsoft Entra ID which represnts the department the employee may be in.

   ![image](https://github.com/user-attachments/assets/f98691f6-9167-45ad-94ae-ed5b0ff542b9)



3. Built a flow in Power Autmate
    - **Step 1: When a new response is submitted** - Triggers the flow automattically when a new hire submits the onboarding form through Microsoft Forms.
   - **Step 2: Get response Details** - The flow captures all of the submitted form data which will be used to create the user.
   - **Step 3: Create user** - A new user is created in Microsoft Entra ID using the form data, and the department they entered places them in the appropriate security group for future access.

   ![image](https://github.com/user-attachments/assets/2a128ee9-2791-407c-b873-2d7b4401b391)



4. Tested the flow by submitting sample data to ensure the user is created in Entra ID with the correct details and placed in the appropriate department.

   ![image](https://github.com/user-attachments/assets/57f49aa6-7aec-42d7-95a2-402d9b9d2bef)



5. After running the test, I verified that the user was successfully created in Entra ID and confirmed they were placed in the correct security group based on the department selected in the form.

   ![image](https://github.com/user-attachments/assets/f18f1d54-a5ed-4915-b5c8-ac2429cd35d9)





