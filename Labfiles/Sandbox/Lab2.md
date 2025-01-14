
#  Lab 2: Using GitHub Codespaces

## Lab Objective 

Set up GitHub Copilot as an AI-powered pair programmer to enhance the coding workflow. Explore GitHub Codespaces, a cloud-hosted development environment, and configure it using Configuration-as-Code. Create a development container, install essential extensions, and add GitHub Copilot to the project. This setup enables AI-driven code suggestions to improve development efficiency.

## Task 1: Enable Copilot inside a Codespace

Enable GitHub Copilot within a Codespace to enhance coding efficiency with AI-powered suggestions. 

1. Now, right-click on your profile icon in the top right and click on **Your Repositories**.
    
    ![](../../media/Copilotrepo.png)

1. Click on the repository named **skills-copilot-codespaces-vscode**

1. In the home page of your repository, click on **Code** **(1)** tab of your repository, click the **Add file** **(2)** drop-down button, and then select `Create new file` **(3)**.

     ![](../../media/dp1u.png)

    - **Note**: If you're unable to see the **Add file** option, click the **+** symbol located next to the **Code** tab.
    
1. Type or paste the following in the empty text field prompt to name your file **(1)**.

    ```
     .devcontainer/devcontainer.json
    ```

1. In the body of the new **.devcontainer/devcontainer.json** file, add the following content **(2)** and click on **Commit changes** **(3)**:

    ```
        {
            // Name this configuration
            "name": "Codespace for Skills!",
            "customizations": {
                "vscode": {
                    "extensions": [
                        "GitHub.copilot"
                    ]
                }
            }
        }
     ```

    ![](../../media/dp2.png)
   
1. Select the option to **Commit directly to the `main` branch**, and then click the **Commit changes** button.

     ![](../../media/commit-file.png)

1. Navigate back to the home page of your repository by clicking the **Code** **(1)** tab located at the top left of the screen. Click the **Code** **(2)** button located in the middle of the page.

     ![](../../media/dp3.png)

1. Click the **Codespaces (1)** tab on the box that pops up and then click the **Create codespace on main (2)** button.

     ![](../../media/dp4.png)

      - **Note**: If in case pop-up prompt doesn't appear in the browser to open Visual Studio code, manually launch Visual Studio code from the desktop and close it. Next, return to the 
    browser, refresh the page and launch the codespace that was previously created.

1. You will encounter a pop-up prompt. Click **Open** to proceed. Subsequently, another pop-up window will appear within Visual Studio Code (VS Code), where you should once again select **Install Extension and Open URI** to continue.

     ![](../../media/open.png)

     ![](../../media/l2.png)

1. At the bottom right corner, you will get a prompt to sign in to GitHub.

    ![](../../media/signingit.png)

     - **Note**: If you do not get a prompt to sign in to your GitHub account, click on the GitHub Copilot icon located in the bottom right corner. Click "Allow" for VS Code to sign in to your GitHub account. A new web page will open. Copy the URL of the page, paste it into a private browser, enter your GitHub credentials, and sign in.

       ![](../../media/githubsignin2.png)
         
     - **Note**: If you face an issue with **Sign in to GitHub**, copy the sigin URL from browser and login to the copied URL from InPrivate browser.
 
       ![](../../media/private.png)

     - **Note**: If you encounter with error **No access to GitHub Copilot found**, please reach out to `cloudlabs-support@spektrasystems.com` for further assistance.
 
       ![](../../media/3.png)
 
1. Next, once you get the popup, click on **Allow**

    ![](../../media/allow.png)

    - **Note**: Wait about 2 minutes for the codespace to spin itself up.

1. Click **Authorize Visual-Studio-Code** once the Authorize GitHub for VS code tab appears in the browser.

1. Verify your codespace is running. Make sure the VS code looks as shown below:

    ![](../../media/loaded-repo.png)

1. Click on **Extensions** **(1)** from the left menu, and the **GitHub Copilot** **(2)** extension should show up in the VS Code extension list. Click the Copilot extension and verify 
   its installation as shown below:

     ![](../../media/verify-copilot.png)

   - **Note**: If the GitHub Copilot extension is not installed, click on Install.

 
> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - If you receive a success message, you can proceed to the next task.
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide. 
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

<validation step="f627a3c6-3d8f-48d4-ae32-306c3ff40e00" />
 
### Summary

In this lab, you have created a development container and added Copilot to the list of extensions.

## You have successfully completed this lab. 
