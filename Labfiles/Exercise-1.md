# Exercise 1: Leverage Codespaces with VS Code for Copilot

Duration: 20 minutes

GitHub Copilot is an AI pair programmer designed to make writing code easier and faster. It draws context from comments and code to suggest individual lines and whole functions instantly. GitHub Copilot is powered by OpenAI Codex, a generative pre-trained language model created by OpenAI.

**Copilot is compatible with a wide range of code editors, such as Neovim, JetBrains IDE, Visual Studio, and VS Code.**

Additionally, GitHub Copilot is trained in every language that can be found in public repositories. The amount and variety of training data for each language may have an impact on the quality of recommendations you obtain.

**GitHub Codespace** is a development environment that's hosted in the cloud. You can customize your project for GitHub Codespaces by committing configuration files to your repository (often known as Configuration-as-Code), which creates a repeatable codespace configuration for all users of your project.

Utilizing Copilot within a Codespace effortlessly demonstrates the simplicity of starting with GitHub’s comprehensive [Collaborative Coding](https://github.com/features#features-collaboration) tools.

In this exercise, you are tasked with creating a development container. You will specify certain extensions or configurations to be utilized or installed in your Codespace. As part of this process, ensure to include Copilot in your list of extensions.

## Task 1: Enable Copilot inside a Codespace

1. Navigate back to the home page of your repository, click on **Code** **(1)** tab of your repository, click the **Add file** **(2)** drop-down button, and then select `+ Create new file` **(3)**.

    ![](../media/Exercise-01-v2-01.png)

2. Type or paste the following in the empty text field prompt to name your file **(1)**.

   ```
   .devcontainer/devcontainer.json
   ```

3. In the body of the new **.devcontainer/devcontainer.json** file, add the following content **(2)** and click on **Commit changes** **(3)**:

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

   ![](../media/devcontainer-commit.png)
   
4. Select the option to **Commit directly to the `main` branch**, and then click the **Commit changes** button.

   ![](../media/commit-file.png)

5. Navigate back to the home page of your repository by clicking the **Code** **(1)** tab located at the top left of the screen. Click the **Code** **(2)** button located in the middle of the page.

   ![](../media/code-code.png)

6. Click the **Codespaces (1)** tab on the box that pops up and then click the **Create codespace on main (2)** button.

   ![](../media/create-codespace.png)

   >**Note**: If in case pop-up prompt doesn't appear in the browser to open Visual Studio code, manually launch Visual Studio code from the desktop and close it. Next, return to the browser, refresh the page and launch the codespace that was previously created.

7. You will encounter a pop-up prompt. Click **Open** to proceed. Subsequently, another pop-up window will appear within Visual Studio Code (VS Code), where you should select **Install Extension and Open URI** to continue.

   ![](../media/open.png)

   ![](../media/innovation-1.png)

    >**Note**: Click on **Allow** if the extension **Github Codepsaces** wants to sign in using Github.

   ![](../media/inn-2.png)

8. At the bottom right corner, you will get a prompt to sign in to GitHub.

   ![](../media/signingit.png)

   > **Note**: If you encounter with error **No access to GitHub Copilot found**, please reach out to `cloudlabs-support@spektrasystems.com` for further assistance.

      ![](../media/3.png)

9. Next, once you get the popup, click on **Allow**

   ![](../media/allow.png)

   >**Note**: Wait about 2 minutes for the codespace to spin itself up.

10. Click **Authorize Visual-Studio-Code** once the Authorize GitHub for VS code tab appears in the browser.

    ![](../media/Exercise-01-v2-02.png)

11. Next, once you get the popup, click on **Allow**

12. Verify your codespace is running. Make sure the VS code looks as shown below:

    ![](../media/loaded-repo.png)

13. Click on **Extensions** **(1)** from the left menu, and the **GitHub Copilot** **(2)** extension should show up in the VS Code extension list. Click the Copilot extension and verify its installation as shown below:

    ![](../media/verify-copilot.png)

   >**Note**: If the GitHub Copilot extension is not installed, click on Install.

 <validation step="2f1521a8-516d-4357-b09c-941c5d7112ad" />
 
14. Click on **Next** below to move on to the next page.

      > **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:

      - Go to the **Lab Validation** tab.
      - Click on the **Validate** button under the **Actions** section for *Exercise 1: Leverage Codespaces with VS Code for Copilot*
      - A success message indicates you’re ready for the next task. Proceed accordingly.
      - If not, review the message, revisit the lab guide, and attempt the step again.
      - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.
        
### Summary

In this exercise, you have created a development container and added Copilot to the list of extensions.
