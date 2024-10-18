# Lab 1: Getting Started with the Lab
 
Welcome to your Github-Copilot workshop! We've prepared a seamless environment for you to explore and learn about Azure services. Let's begin by making the most of this experience:
 
## **Accessing Your Lab Environment**
 
Once you're ready to dive in, your virtual machine and lab guide will be right at your fingertips within your web browser.
 
 ![](../../media/getstart324.png)

### **Virtual Machine & Lab Guide**
 
Your virtual machine is your workhorse throughout the workshop. The lab guide is your roadmap to success.
 
## **Exploring Your Lab Resources**
 
To get a better understanding of your lab resources and credentials, navigate to the **Environment** Details tab.
 
   ![](/media/enviornment.png)
 
## **Utilizing the Split Window Feature**
 
For convenience, you can open the lab guide in a separate window by selecting the **Split Window** button from the Top right corner.
 
   ![](/media/higher.png)
  
## Login to GitHub

1. In the LABVM desktop search for **Microsoft Edge** **(1)**, click on **Microsoft Edge** **(2)** browser.

   ![](/media/Edge.png)

1. Navigate to GitHub login page using the provided URL below:
   ```
   https://github.com/login
   ```
   
1. On the **Sign in to GitHub** tab, you will see the login screen. In that screen, enter the  **email** **(1)** and **password** **(2)**. Then click on **Sign in** **(3)**. 

   ![](/media/github-login.png)
          
   >**Note:** To view the GitHub credentials, access the lab named **GitHub Copilot Lab: GitHub Credentials**, which is present within the First learning path of this course.

      ![](/media/credsfile.png)
   
   >**Note:** If you're unable to copy the username and password, please type them manually to proceed further.
   
1. Navigate to Outlook login page using the provided URL below:
   ```
   https://outlook.office365.com/mail/
   ```
1. Next, to get the authentication code, sign in to Outlook with the git credentials within the Environment tab from the previous step. Once you have logged into Outlook, find the recent email containing the verification code. Enter the verification code, and click on **Verify**.

   >**Note:** The email containing the verification code can somtimes creep into the archive/spam folders within your Outlook.

   ![](/media/authgit.png)

1. Copy the below link and navigate to the link inside LabVM in the Edge browser where you have logged into GitHub in the previous steps.

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
   
   ```
    https://github.com/new?template_owner=skills&template_name=copilot-codespaces-vscode&owner=%40me&name=skills-copilot-codespaces-vscode&description=My+clone+repository&visibility=public
   ```   
1. In the new tab, most of the prompts will automatically fill in for you. Make sure the  repository name is  **skills-copilot-codespaces-vscode**, and leave the default for the owner, as you have already logged into GitHub to host the repository **(1)**. Select **Public** repository **(2)** and click the **Create repository** **(3)** button at the bottom of the form.

   ![](/media/skills-new-repo.png)

1. After your new repository is created, wait about 20 seconds and then refresh the page.

    >**Note**: If you get a note  prompting that a repository with the name **skills-copilot-codespaces-vscode** already exists, please delete the existing one by performing the below steps and perform the above step again.
    > - On GitHub.com, navigate to the main page of the repository.
    > - Under your repository name, click  Settings. If you cannot see the "Settings" tab, select the  dropdown menu, then click Settings.
    
      ![](/media/2.png)

    > - On the **General** settings page (which is selected by default), scroll down to the "Danger Zone" section and click **Delete this repository**.
     
      ![](/media/4.png)

    > - Click **I want to delete this repository**.
 
      ![](/media/5.png)

    > - Read the warnings and click **I have read and understand these effects**.

      ![](/media/6.png)

    >  - To verify that you're deleting the correct repository, in the text box, type the name of the repository you want to delete.

    >  - Click **Delete this repository**.

      ![](/media/7.png)

1. Once the repository is created, click on your profile picture and then select **Your organizations**.

   ![](/media/organization.png)

1. In "Your organization", from the left navigation pane, select **Codespaces**.

   ![](/media/codespace.png)

1. Scroll down and make sure, **Visual Studio Code** is selected, under the **Editor preference** .

   ![](/media/vscode1.png)

    > **Congratulations** on completing the lab! Now, it's time to validate it. Here are the steps:
    > - On GitHub, locate your profile photo at the top right corner of the screen
    > - Hit the Validate button for the corresponding task. Paste your Organization name into the required field and click on submit.

    ![Picture1](/media/github-copilot-new-2.png)

    > - If you receive a success message, you can proceed to the next task. 
    > - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
    > - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

      <validation step="74f9ec11-59d4-4a33-928f-4ab2220edbd9" />

## Summary

In this lab, you'll learn how to log into GitHub and create a new repository. By the end, you'll have a new repository ready for your projects.

## You have successfully completed this lab.

