# GitHub Copilot Innovation Workshop

## Getting Started with Lab

1. You can see a virtual machine desktop 💻 (**LABVM**) is loaded on the left side in your browser. Use this virtual machine throughout the workshop to perform the lab. You can also connect to the virtual machine using any RDP client using the **LABVM** credentials provided in the **Environment Details** tab.

   ![](../media/sqlarcLABVM.png) 
   
   >Note: If you see any PowerShell windows running in your VM, please do not close that as it's setting up some configurations inside the environment.
 
1. To get the lab environment details, you can select the **Environment Details** tab. Additionally, the credentials will also be emailed to your registered email address. You can also open the Lab Guide in a separate and full window by selecting the **Split Window** from the lower right corner. Also, you can start, stop and restart virtual machines from the **Resources** tab.

   ![](../media/getstartpage02.png "Enter Email")
 
   > You will see the SUFFIX value on the **Environment Details** tab, use it wherever you see SUFFIX or DeploymentID in lab steps.
 
## Login to GitHub

1. In the JumpVM, click on the Microsoft Edge browser and navigate to GitHub login page .

   ```
   https://github.com/login
   ```

   ![](media/getstartpage03.png)
   
1. On the **Sign in to GitHub** tab you will see the login screen, in that enter the following **email/username** **(1)** and **password** **(2)**. Then click on **Sign in** **(3)**. 

   * **Email/Username**: <inject key="AzureAdUserEmail"></inject>
   * **Password**: <inject key="AzureAdUserPassword"></inject>
   
   ![](media/github-login.png)
          
1. Right-click on **Start course** and click on **open the link in a new tab**.

   <!-- For start course, run in JavaScript:
   'https://github.com/new?' + new URLSearchParams({
     template_owner: 'skills',
     template_name: 'copilot-codespaces-vscode',
     owner: '@me',
     name: 'skills-copilot-codespaces-vscode',
     description: 'My clone repository',
     visibility: 'public',
   }).toString()
   -->

   [![Start course](https://user-images.githubusercontent.com/1221423/235727646-4a590299-ffe5-480d-8cd5-8194ea184546.svg)](https://github.com/new?template_owner=skills&template_name=copilot-codespaces-vscode&owner=%40me&name=skills-copilot-codespaces-vscode&description=My+clone+repository&visibility=public)
   
1. In the new tab, most of the prompts will automatically fill in for you. Leave defult for owner as you have already logged into GitHub to host the repository **(1)**. Select **Public** repository **(2)** and click the **Create repository** **(3)** button at the bottom of the form.

   ![](media/skills-new-repo.png)

1. After your new repository is created, wait about 20 seconds and then refresh the page.

1. Now, click on **Next** from the lower right corner to move on to the next page.
