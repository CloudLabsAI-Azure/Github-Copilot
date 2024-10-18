# Lab 4: Using GitHub Copilot to generate ARM & Terraform Templates

### About GitHub Copilot Chat and Visual Studio Code

GitHub Copilot Chat allows you to ask coding questions and receive answers directly within the supported IDE. Copilot Chat can help you with a variety of coding-related tasks, like offering you code suggestions, providing natural language descriptions of a piece of code's functionality and purpose, generating unit tests for your code, and proposing fixes for bugs in your code. For more information, see "[About GitHub Copilot Chat](https://docs.github.com/en/copilot/github-copilot-chat/about-github-copilot-chat)."

### Use cases for GitHub Copilot Chat

There are several situations in which GitHub Copilot Chat can help with coding.

 - Generating unit test cases
 - Explaining code
 - Proposing code fixes
 - Answering coding questions

In this lab, you will utilize Copilot to generate code in ARM, Terraform, and PowerShell.

> **Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in gray text. Examples of what you'll most likely see in this exercise, but the exact suggestion may vary.

### Task 1: Generate code by chat that uses ARM to deploy resources to Azure

1. In the LABVM desktop search for **Microsoft Edge** **(1)**, click on **Microsoft Edge** **(2)** browser.

   ![](/media/Edge.png)

1. Navigate to GitHub login page using the provided URL below:
   ```
   https://github.com/login
   ```
   
1. On the **Sign in to GitHub** tab, you will see the login screen. In that screen, enter the  **email** **(1)** and **password** **(2)**. Then click on **Sign in** **(3)**. 

   ![](/media/github-login.png)

     >**Note:** To view the GitHub credentials, Navigate to the **Environment** tab to view the key-value pairs of the **GitHub UserEmail**, and **GitHub Password**. You can use the copy buttons under the actions column to have the values copied instantly.

     ![](/media/envt12.png)

    >**Note:** If you're unable to copy the username and password, please type them manually to proceed further.
     
1. Navigate to Outlook login page using the provided URL below:
   ```
   https://outlook.office365.com/mail/
   ```
1. Next, to get the authentication code, sign in to Outlook with the git credentials within the Environment tab from the previous step. Once you have logged into Outlook, find the recent email containing the verification code. Enter the verification code, and click on **Verify**.

   >**Note:** The email containing the verification code can somtimes creep into the archive/spam folders within your Outlook.

   ![](/media/authgit.png)

1. Now, right-click on your profile icon in the top right and click on **Your Repositories**.
    
   ![](/media/l2.2.png)

1. Click on the repository named **skills-copilot-codespaces-vscode**.

1. Navigate back to the home page of your repository by clicking the **Code** **(1)** tab located at the top left of the screen. Click the **Code** **(2)** button located in the middle of the page.

   ![](/media/code-code.png)

1. Click the **Codespaces (1)** tab on the box that pops up and then click the **+ (2)** button.

   ![](/media/labgit.png)

   >**Note**: If in case pop-up prompt doesn't appear in the browser to open Visual Studio code, manually launch Visual Studio code from the desktop and close it. Next, return to the browser, refresh the page and launch the codespace that was previously created.

1. You will encounter a pop-up prompt. Click **Open** to proceed. Subsequently, another pop-up window will appear within Visual Studio Code (VS Code), where you should once again select **Install and Open** to continue.

   ![](/media/open.png)

   ![](/media/codespaces.png)

1. At the bottom right corner, you will get a prompt to sign in to GitHub.

   ![](/media/signingit.png)

   >**Note:** If you do not get the sign-in prompt within Visual Studio Code, click on **Allow** in the pop-up that appears which will open a window in the browser, refresh the screen and click on **Open** in the pop-up that appears.

1. Next, once you get the popup, click on **Allow**

   ![](/media/allow.png)

   >**Note**: Wait about 2 minutes for the codespace to spin itself up.

1. Verify your codespace is running. Make sure the VS code looks as shown below:

   ![](/media/loaded-repo.png)

1. Click on **Extensions** **(1)** from the left menu, and the **GitHub Copilot** **(2)** extension should show up in the VS Code extension list. Click the Copilot extension and verify its installation as shown below:

   ![](/media/verify-copilot.png)

1. In the "Search Extensions in Marketplace" search box, type and search for the **GitHub Copilot Chat** extension.

1. Select **GitHub Copilot Chat** from the list of results that show up, and verify that **GitHub Copilot Chat** has been installed.
   
1. If not, click on the **Install** button.

    ![](/media/ghc-chat-extension.png)

1. Once the installation is complete, in the left navigation pane you will able to see the icon for GitHub Copilot Chat as shown below.

   ![](/media/git-chat-icon.png)

## Task 3.1- Example: Set the stage with a high-level goal

   >**Note**: If the GitHub Copilot extension is not installed, click on Install.

1. In the Visual Studio Code activity bar, click the GitHub Copilot Chat icon to open the GitHub Copilot Chat window.

1. At the bottom of the GitHub Copilot Chat window, in the **Ask Copilot a question or type / for topics** text box, type a coding-related question, then press Enter. For example, type "Write an ARM code for deploying a storage account to Azure with the code explanation."

    ![](/media/create-arm.png)

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window. 

    ![](/media/arm-output1.png)

    ![](/media/arm-output2.png)   

    > **Note:** Here's an example of what you are likely to see; however, the precise recommendation could vary.

    > **Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    > **Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can view the response from GitHub Copilot in the chat. To insert code into a new file, click on **Ellipsis (...)** **(1)** and select **Insert Into New File** **(2)**.

   ![](/media/arm-new-file.png)

1. Press `CTRL + S` to save the file. Name the file `arm.json` and click on **OK**

   ![](/media/arm-save.png)

### Task 2: Generate code by chat that uses Terraform to deploy resources to Azure

1. In the Visual Studio Code activity bar, click the GitHub Copilot Chat icon to open the GitHub Copilot Chat window.

1. At the bottom of the GitHub Copilot Chat window, in the **Ask Copilot a question or type / for topics** text box, type a coding-related question, then press Enter. For instance, type "Write a Terraform code for deploying a storage account to Azure with the code explanation".

   ![](/media/create-terraform.png)

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window.

    ![](/media/terraform.png)

    > **Note:** Here's an example of what you are likely to see; however, the precise recommendation could vary.
    
    > **Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    > **Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can view the response from GitHub Copilot in the chat. To insert code into a new file, click on **Ellipsis (...)** **(1)** and select **Insert Into New File** **(2)**.

   ![](/media/terraform-new-file.png)

1. Press `CTRL + S` to save the file. Name the file `terraform.tf` and click on **OK**

   ![](/media/terraform-save.png)

### Task 3: Generate code by chat that uses PowerShell to deploy resources to Azure

1. In the Visual Studio Code activity bar, click the GitHub Copilot Chat icon to open the GitHub Copilot Chat window.

1. At the bottom of the GitHub Copilot Chat window, in the **Ask Copilot a question or type / for topics** text box, type a coding-related question, then press Enter. For example, type "Write a PowerShell script for deploying a storage account to Azure."

   ![](/media/create-powershell.png)

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window. 

    ![](/media/ps-output.png)

    > **Note:** Here's an example of what you are likely to see; however, the precise recommendation could vary.

    > **Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    > **Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can view the response from GitHub Copilot in the chat. To insert code into a new file, click on **Ellipsis (...)** **(1)** and select **Insert Into New File** **(2)**.

   ![](/media/ps-newfile.png)

1. Press `CTRL + S` to save the file. Name the file `powershell.ps1` and click on **OK**.

   ![](/media/ps-save.png)

### Task 4: Push code to your repository from the codespace

1. Use the VS Code terminal to add files to the repository. Open VS Code Terminal if it's not opened yet.

1. Run the below command to add the `arm.json` , `terraform.tf` and `powershell.ps1` files to the repository:

   ```
   git add arm.json terraform.tf powershell.ps1
   ```

1. Next, from the VS Code terminal stage, commit the changes to the repository:

   ```
   git commit -m "Copilot third commit"
   ```

1. Finally, from the VS Code terminal, push to code to the repository:

   ```
   git push
   ```

   ![](/media/ex-4-push5.png)

   >**Note**: Wait about 60 seconds, then refresh your repository landing page for the next step.

1. You can verify the `arm.json`, `powershell.ps1`, and `terraform.tf` files available in your GitHub repository.

   ![](/media/ex-4-github5.png)

    

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - If you receive a success message, you can proceed to the next task.
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide. 
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

<validation step="f58c599c-cef0-44ef-858b-2b35ffd4cc6e" />

  
### Summary

In this lab, you have employed Copilot to automatically generate code in both ARM, Terraform, and PowerShell programming languages.

