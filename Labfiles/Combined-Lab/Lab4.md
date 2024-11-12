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

## Task 1- Example: Set the stage with a high-level goal

   >**Note**: If the GitHub Copilot extension is not installed, click on Install.

1. In the Visual Studio Code activity bar, click the GitHub Copilot Chat icon to open the GitHub Copilot Chat window.

1. At the bottom of the GitHub Copilot Chat window, in the **Ask Copilot a question or type / for topics** text box, type a coding-related question, then press Enter. For example, type "Write an ARM code for deploying a storage account to Azure with the code explanation."

    ![](../../media/g2.png)

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window. 

    ![](../../media/arm-output1.png)

    ![](../../media/arm-output2.png)   

    > **Note:** Here's an example of what you are likely to see; however, the precise recommendation could vary.

    > **Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    > **Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can review the response from GitHub Copilot in the chat. To insert code into a new file, click on **Ellipsis (...)** **(1)** and select **Insert Into New File** **(2)**.

   ![](../../media/arm-new-file.png)

1. Press `CTRL + S` to save the file. Name the file `arm.json` and click on **OK**

   ![](../../media/arm-save.png)

### Task 2: Generate code by chat that uses Terraform to deploy resources to Azure

1. Back in the Chat window, let us try to generate a terraform code. Enter for instance, type "Write a Terraform code for deploying a storage account to Azure with the code explanation" and hit enter.

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window.

    ![](../../media/terraform.png)

    > **Note:** Here's an example of what you are likely to see; however, the precise recommendation could vary.
    
    > **Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    > **Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can review the response from GitHub Copilot in the chat. To insert code into a new file, click on **Ellipsis (...)** **(1)** and select **Insert Into New File** **(2)**.

   ![](../../media/terraform-new-file.png)

1. Press `CTRL + S` to save the file. Name the file `terraform.tf` and click on **OK**

   ![](../../media/terraform-save.png)

### Task 3: Generate code by chat that uses PowerShell to deploy resources to Azure

1. Back in the Chat window, let us try to generate a powershell script.For example, type "Write a PowerShell script for deploying a storage account to Azure." and hit enter.

   ![](../../media/g3.png)

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window. 

    ![](../../media/ps-output.png)

    > **Note:** Here's an example of what you are likely to see; however, the precise recommendation could vary.

    > **Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    > **Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can view the response from GitHub Copilot in the chat. To insert code into a new file, click on **Ellipsis (...)** **(1)** and select **Insert Into New File** **(2)**.

   ![](../../media/ps-newfile.png)

1. Press `CTRL + S` to save the file. Name the file `powershell.ps1` and click on **OK**.

   ![](../../media/ps-save.png)

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

   ![](../../media/ex-4-push5.png)

   >**Note**: Wait about 60 seconds, then refresh your repository landing page for the next step.

1. You can verify the `arm.json`, `powershell.ps1`, and `terraform.tf` files available in your GitHub repository.

   ![](../../media/ex-4-github5.png)
    
1. On the GitHub page, locate your profile icon at the top right corner of the screen and click on **Your Profile** option.

1. Copy your GitHub username in order to validate your lab.

   ![](../../media/gc2.png)
  
    > **Congratulations** on completing the lab! Now, it's time to validate it. Here are the steps:
    >  - Hit the Validate button for the corresponding task. Paste the GitHub username (1) you copied in the previous step and click on **Submit**(2).
       
      ![Picture1](../../media/github-copilot-new-2.png)
    
    > - If you receive a success message, you can proceed to the next task. 
    > - If not, carefully read the error message and retry the step, following the instructions in the lab guide.
    > - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

<validation step="24e51569-e264-40ac-b8f3-a565cdd84341" />

  
### Summary

In this lab, you have employed Copilot to automatically generate code in both ARM, Terraform, and PowerShell programming languages.

## You have successfully completed this lab. 
