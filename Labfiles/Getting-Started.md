# Getting Started with the Lab

### Estimated Duration: 10 minutes

## Exercises Overview

**Exercise 1: Leverage Codespaces with VS Code for Copilot**: GitHub Copilot, powered by OpenAI Codex, speeds up coding with contextual suggestions across various editors, while GitHub Codespaces provides consistent, cloud-hosted development setups.

**Exercise 2: Exploring AI-Driven Code Suggestions in JavaScript** examines how AI enhances JavaScript coding with real-time completions, bug detection, optimizations, and efficiency improvements.

**Exercise 3: Exploring Python with GitHub Copilot: Intelligent Code Suggestionst**: GitHub Copilot offers excellent suggestions for languages like Python, JavaScript, Ruby, and more, and assists with database queries.

**Exercise 4: Using GitHub Copilot Chat to generate ARM and Terraform code with Copilot**: GitHub Copilot Chat provides coding assistance directly within supported IDEs, offering code suggestions, explanations, unit tests, and bug fixes.

**Exercise 5: Using GitHub Copilot for Code Refactoring**: GitHub code refactoring enhances code quality by restructuring for readability, maintainability, and performance without altering external behavior, reducing technical debt and bugs.

**Exercise 6: Using IDEs such as JetBrains IntelliJ for Java**: GitHub Copilot enhances Java coding in IntelliJ by offering intelligent suggestions and auto-completion, elevating productivity and code quality.

**Exercise 7: Enhancing Web Accessibility with GitHub Copilot Chat and Accessibility Insights**: GitHub Copilot Chat accelerates coding with AI-powered suggestions, while Accessibility Insights for Web ensures inclusive, accessible web content.

**Exercise 8: Using GitHub Copilot for T-SQL and YAML Code [Optional]**: Leverage GitHub Copilot to generate code in T-SQL and YAML, using comments to guide its suggestions.

**Exercise 9: Generating Documentation Using GitHub Copilot [Optional]**: GitHub Copilot streamlines documentation by auto-generating comments, Markdown, and ensuring consistency, enhancing project accessibility.

**Exercise 10: Working with the Copilot for Machine Learning [Optional]**: Using GitHub Copilot for machine learning involves installing it, linking to GitHub for repository access, and utilizing it with ML frameworks for tasks such as data preprocessing, model building, and evaluation.

**Exercise 11: Creating a Mini Game with GitHub Copilot [Optional]**: You'll use GitHub Copilot to build a classic rock, paper, scissors game, refining Python skills in console app development.

### Getting Started with the Lab

1. You can see a virtual machine desktop 💻 (**LABVM**) loaded on the left side of your browser. Use this virtual machine throughout the workshop to perform the lab. You can also connect to the virtual machine using any RDP client using the **LABVM** credentials provided in the **Environment** tab.
   
   ![](../media/gettingstarted-v2-first.png)

1. Once you are in the **Environment** tab click on the **GitHub Credentials** option to get GitHub user credentials. The credentials will also be emailed to your registered email address. You can also open the Lab Guide in a separate, and full window by selecting **Split Window** from the upper right corner. Also, you can start, stop, and restart virtual machines from the **Resources** tab.
 
   ![](../media/gettingstarted-v2-01.png)
 
## Login to GitHub

1. In the LABVM desktop search for **Microsoft Edge** **(1)**, click on **Microsoft Edge** **(2)** browser.

   ![](../media/Edge.png)

1. Navigate to GitHub login page using the provided URL below:
   ```
   https://github.com/login
   ```
   
1. On the **Sign in to GitHub** tab, you will see the login screen. In that screen, enter the following **email** **(1)** and **password** **(2)**. Then click on **Sign in** **(3)**. 

   >**Note**: To get GitHub credentials navigate to the **Environment** tab and click on the **GitHub Credentials** option to view the key-value pairs of the **GitHub UserEmail**, and **GitHub Password**. You can use the copy buttons under the actions column to have the values copied instantly. Alternatively, it is suggested to have the values copied over onto a notepad for easy accessibility. 
   
   ![](../media/github-login.png)
          
1. Next, to get the authentication code, sign in to Outlook (https://outlook.office365.com/mail/) with the git credentials within the Environment tab from the previous step. Once you have logged into Outlook, find the recent email containing the verification code. Enter the verification code and click on **Verify**.

   >**Note:** The email containing the verification code can sometimes creep into the archive/spam folders within your Outlook.

   ![](../media/authgit.png)

1. Right-click on the **Start course** given below, click on the **Copy link**, and navigate to the link inside LabVM in the Edge browser where you have logged into GitHub in the previous steps.

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
   
1. In the new tab, most of the prompts will automatically fill in for you. Leave default for the owner, as you have already logged into GitHub to host the repository **(1)**. Select **Public** repository **(2)** and click the **Create repository** **(3)** button at the bottom of the form.

   ![](../media/skills-new-repo.png)

1. If the repository already exists, please delete the existing one and perform the above step again. To delete the repository, 
follow from step 08 to step 12. In the absence of an existing repository, skip to step 13.

1. Navigate to the existing repository that must be deleted

   ![](../media/gs-6.png)
   
   ![](../media/gs-5.png)
      
1. Click on **Settings**.

     ![](../media/gs-1.png)

1. Scroll down to the **Danger Zone** pane and click on **Delete this repository**.

     ![](../media/gs-2.png)

1. Click on **I want to delete this repository** and accept that you have read and understood the effects.

     ![](../media/gs-3.png)

1. Give the name of the repository and click on **Delete this repository**.

     ![](../media/gs-4.png)

1. After your new repository is created, wait about 20 seconds and then refresh the page.

1. Once the repository is created, click on your profile picture and then select **Your organizations**.

   ![](../media/organization.png)

1. In Your organization, select **Codespaces** from the left navigation pane.

   ![](../media/codespace.png)

1. Scroll down and make sure, **Visual Studio Code** is selected, under the **Editor preference** .

     ![](../media/vscode1.png)

1. Now, click on **Next** from the lower right corner to move on to the next page.
