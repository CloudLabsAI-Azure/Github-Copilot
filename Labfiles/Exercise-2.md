# Exercise 2: Leverage Codespaces with VS Code for Copilot

### Task 1: Enable Copilot inside a Codespace

**We recommend opening another browser tab to work through the following activities so you can keep these instructions open for reference.**

Before you open up a codespace on a repository, you can create a development container and define specific extensions or configurations that will be used or installed in your codespace. Let's create this development container and add copilot to the list of extensions.

1. Navigating back to your **Code** tab of your repository, click the **Add file** drop-down button, and then click `Create new file`.
1. Type or paste the following in the empty text field prompt to name your file.
   ```
   .devcontainer/devcontainer.json
   ```
1. In the body of the new **.devcontainer/devcontainer.json** file, add the following content:
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
1. Select the option to **Commit directly to the `main` branch**, and then click the **Commit new file** button.
1. Navigate back to the home page of your repository by clicking the **Code** tab located at the top left of the screen.
1. Click the **Code** button located in the middle of the page.
1. Click the **Codespaces** tab on the box that pops up.
1. Click the **Create codespace on main** button.

   **Wait about 2 minutes for the codespace to spin itself up.**

1. Verify your codespace is running. The browser should contain a VS Code web-based editor and a terminal should be present such as the below:
   ![Screen Shot 2023-03-09 at 9 09 07 AM](https://user-images.githubusercontent.com/26442605/224102962-d0222578-3f10-4566-856d-8d59f28fcf2e.png)
1. The `copilot` extension should show up in the VS Code extension list. Click the extensions sidebar tab. You should see the following:
   ![Screen Shot 2023-03-09 at 9 04 13 AM](https://user-images.githubusercontent.com/26442605/224102514-7d6d2f51-f435-401d-a529-7bae3ae3e511.png)

**Wait about 60 seconds then refresh your repository landing page for the next step.**

