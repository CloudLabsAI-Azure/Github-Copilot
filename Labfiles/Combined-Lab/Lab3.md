# Lab 3: Code Suggestions with GitHub Copilot in Codespaces using VS Code

Duration: 30 minutes

While GitHub Copilot offers recommendations for many languages and frameworks, it excels in particular when it comes to Python, JavaScript, TypeScript, Ruby, Go, C#, and C++. The samples below are in JavaScript, but they should also work in other languages.

In this lab, you will have the opportunity to experiment with and apply JavaScript with the assistance of GitHub Copilot and GitHub Copilot Chat.

>**Disclaimer**: A whole function body will be automatically suggested by GitHub Copilot in gray text. Here's an example of what you are likely to see; however, the precise recommendation could vary.If you do not see code recommendation, try adding a space after the code. 

## Task 1: Add a JavaScript file and start writing code.

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

   >**Note:** The email containing the verification code can sometimes creep into the archive/spam folders within your Outlook.

   ![](/media/authgit.png)

1. Now,right click on your profile icon in the top right and click on **Your Repositories**.
    
   ![](/media/l2.2.png)

1. Click on the repository named **skills-copilot-codespaces-vscode**.

1. Navigate back to the home page of your repository by clicking the **Code** **(1)** tab located at the top left of the screen. Click the **Code** **(2)** button located in the middle of the page.

   ![](/media/dp3.png)

1. Click the **Codespaces (1)** tab on the box that pops up and then click the **+ (2)** button.

   ![](/media/labgit.png)

   >**Note**: If in case pop-up prompt doesn't appear in the browser to open Visual Studio code, manually launch Visual Studio code from the desktop and close it. Next, return to the browser, refresh the page and launch the codespace that was previously created.

1. You will encounter a pop-up prompt. Click **Open** to proceed. Subsequently, another pop-up window will appear within Visual Studio Code (VS Code), where you should once again select **Install Extension and Open URI** to continue.

   ![](/media/open.png)

   ![](/media/l2.png)

1. At the bottom right corner, you will get a prompt to sign in to GitHub.

   ![](/media/signingit.png)

   >**Note:** If you do not get the sign-in prompt within Visual Studio Code, click on **Allow** in the pop-up that appears which will open a window in the browser, refresh the screen and click on **Open** in the pop-up that appears.

1. Next, once you get the popup, click on **Allow**

   ![](/media/allow.png)

   >**Note**: Wait about 2 minutes for the codespace to spin itself up.

1. Click **Authorize Visual-Studio-Code** once the Authorize GitHub for VS code tab appears in the browser.

1. Verify your codespace is running. Make sure the VS code looks as shown below:

   ![](/media/loaded-repo.png)

1. Click on **Extensions** **(1)** from the left menu, and the **GitHub Copilot** **(2)** extension should show up in the VS Code extension list. Click the Copilot extension and verify its installation as shown below:

   ![](/media/verify-copilot.png)

   >**Note**: If the GitHub Copilot extension is not installed, click on Install.

1. From the VS Code Explorer window, create a New File.

   ![](/media/create-newfile.png)

2. Name the file `skills.js` and verify your new file looks as shown below:

   ![](/media/name-skills.png)

3. In the `skills.js` file, type the following function header:

   ```
   function calculateNumbers(var1, var2)
   ```
   
   > **Note**: A whole function body will be automatically suggested by GitHub Copilot in gray text. Here's an example of what you are likely to see; however, the precise recommendation could vary. If you do not see code recommendation, try adding a space after the code. 

   ![](/media/skills-function.png)

4. Press `Tab` to accept the suggestion and then press `Ctrl + S` to save the file.

   ![](/media/save-skills.png)

## Task 2: Push code to your repository from the codespace

In this task, you will use the VS Code terminal to add the `skills.js` file to the GitHub repository.

1. Open VS Code Terminal by clicking on **Ellipsis (...)** **(1)**, select **Terminal** **(2)** and click on **New Terminal** **(3)**.

   ![](/media/open-terminal.png)

2. Run the below command to add the `skills.js` file to the GitHub repository.

   ```
   git add skills.js
   ```

3. Next, from the VS Code terminal stage, commit the changes to the repository:

   ```
   git commit -m "Copilot first commit"
   ```

4. Finally, from the VS Code terminal, push the code to the repository:

   ```
   git push
   ```

   ![](/media/skills-push.png)

   >**Note**: Wait about 60 seconds, then refresh your GitHub repository landing page for the next step.


## Task 3: Best practices to use GitHub Copilot

### Verify GitHub Copilot Chat extension in VS Code

1. To Verify the GitHub Copilot Chat extension, the following steps are to be performed within Visual Studio Code:
    - Click on the **Extensions (1)** icon in the activity bar present on the left side of the Visual Studio Code Window.
    - In the "Search Extensions in Marketplace" search box, type and search for the **GitHub Copilot Chat (2)** extension.
    - Select **GitHub Copilot Chat (3)** from the list of results that show up, and verify that **GitHub Copilot Chat** has been installed.
    - If not, click on the **Install (4)** button.

      ![](/media/ghc-chat-extension.png)

1. Once the installation is complete, in the left navigation pane you will able to see the icon for GitHub Copilot Chat as shown below.

   ![](/media/git-chat-icon.png)

## Task 3.1- Example: Set the stage with a high-level goal

This is most helpful if you have a blank file or an empty codebase. In other words, it can be quite helpful to set the stage for the AI pair programmer if GitHub Copilot has no idea what you want to build or achieve. It helps to prime GitHub Copilot with a big-picture description of what you want it to generate—before you jump in with the details.

When prompting GitHub Copilot, think of the process as having a conversation with someone: How should I break down the problem so we can solve it together? How would I approach pair programming with this person?

1. From the VS Code Explorer window, create a New File.

   ![](/media/E2-T3.1-S1.png)

2. Name the file `index.js` and verify your new file looks as shown below:

   ![](/media/E2-T3.1-S2.png)

3. Now press `Ctrl + I` to open the GitHub Copilot Chat and paste the following **comments (1)** to create a basic markdown editor and click on **Make request (Enter) (2)** button.

   ```
   /*
   Create a basic markdown editor in Next.js with the following features:
   - Use react hooks
   - Create a state for markdown with the default text "type markdown here"
   - A text area where users can write markdown 
   - Show a live preview of the markdown text as I type
   - Support for basic markdown syntax like headers, bold, and italics 
   - Use React markdown npm package 
   - The markdown text and resulting HTML should be saved in the component's state and updated in real-time 
   */
   ```

   ![](/media/ex2-markdown.png)

4. This will prompt GitHub Copilot to generate the following code in the image and produce a very simple, unstyled, but functional markdown editor.

   ![](/media/ex2-markdown-output.png)


## Task 3.2- Example: Aim to receive a short output from GitHub Copilot for a simple and specific ask

After you've explained your primary objective to the AI pair programmer, explain the reasoning and procedures it must take to reach that objective. This will help GitHub Copilot gain a clearer understanding of your intended outcome when you break things down. For example, imagine you’re writing a recipe. Rather than writing a paragraph outlining the food you intend to make, you would break down the cooking procedure into distinct parts.
So, instead of asking GitHub Copilot to generate a large amount of code at once, let it generate the code after each step.

1. In the same index.js file, enter the below step-by-step instructions for reversing a sentence.

    ```
      // take a sentence as input
      // reverse the input sentence
      // the start of the sentence must start with a capital
      // for javascript
    ```

2. The generated outcome would look similar to the below image.

   ![](/media/ex2-reverse-sentence-output.png)


## Task 3.3- Example: Give GitHub Copilot an example or two

Not only can people benefit from learning from examples, but so can your AI pair programmer. For example, in order to take the names out of the data array below and put them in a
new array:

   ```
          const data = [
        [
          { name: 'John', age: 25 },
          { name: 'Jane', age: 30 }
        ],
        [
          { name: 'Bob', age: 40 }
        ]
      ];    
   ```

1. Type the below comment in the chat to generate the output without showing an example to GitHub Copilot.

   ```
    // As an illustration, pull names out of the data array  
   ```

2. It generated an incorrect usage of the map.

   ![](/media/ex2-array-output.png)

3. By contrast, type the below comments to provide an example of how to generate the desired output.

    ```
      // Map through an array of arrays of objects
      // Example: Extract names from the data array
      // Desired outcome: ['John', 'Jane', 'Bob']    
    ```

4. Now, we have received our desired outcome.

   ![](/media/ex2-array-output-1.png)

5. Open the **New Terminal** **(3)** to push the code.

6. Run the below command to pull the latest changes.

   ```
   git pull
   ```

1. Run the below command to add the `index.js` file to the GitHub repository.
   
   ```
   git add index.js
   ```

8. Next from the VS Code terminal, commit the changes to the repository:

   ```
   git commit -m "Copilot commit"
   ```

9. Finally, from the VS Code terminal, push the code to the repository:

   ```
   git push
   ```

   >**Note**: Wait about 60 seconds, then refresh your GitHub repository landing page for the next step.

> **Congratulations** on completing the task! Now, it's time to validate it. Here are the steps:
> - If you receive a success message, you can proceed to the next task.
> - If not, carefully read the error message and retry the step, following the instructions in the lab guide. 
> - If you need any assistance, please contact us at labs-support@spektrasystems.com. We are available 24/7 to help you out.

<validation step="8a55bd72-560d-4d18-ad97-4dfd336658db" />
 
### Summary

In this lab, you have successfully generated JavaScript code and other best practices using GitHub Copilot and GitHub Copilot Chat.

