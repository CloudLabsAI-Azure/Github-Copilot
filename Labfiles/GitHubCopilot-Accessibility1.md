# Exercise 11: GitHub Copilot + Accessibility Insights for Web

Duration: 90 minutes

**GitHub Copilot Chat** is an AI-powered code completion tool that helps developers by suggesting code snippets and solutions based on context. This tool can significantly speed up the development process by providing relevant code suggestions and automating repetitive tasks.

**Accessibility Insights for Web** is a powerful, user-friendly tool that helps make web content accessible to all users, including those with disabilities. By integrating this tool into the development and testing process, web developers can ensure their websites meet accessibility standards, enhancing usability and inclusivity.

Accessible University (AU) is a fictional university home page designed to demonstrate a variety of common web design problems that result in visitors with disabilities being unable to access content or features.

Use the AU site to:

1. Demonstrate common web accessibility principles at trainings, presentations, and workshops on accessible web design.
   
1. Learn common web accessibility problems and solutions in an easy-to-understand way.

In this exercise, you will use Accessibility Insights for Web to identify accessibility issues on a sample website and then employ GitHub Copilot Chat to generate and implement code fixes for these issues. The target website, Accessible University (AU), is a fictional homepage designed to showcase common web design problems that hinder accessibility. By the end of this exercise, you will have enhanced the accessibility of the AU site, making it more user-friendly for individuals with disabilities.

## Task 1: Set Up Accessibility Insights for Web extension in Microsoft Edge

1. Navigate to the **Accessibility Insights for Web** page using the provided URL below:
   
     ```
    https://accessibilityinsights.io/docs/web/overview/
     ```
     
1. From the Accessibility Insights for Web page, click on the **Download for Web** option.

   ![](../media/aut11.png)

1. Click the **+ Add to Microsoft Edge** button from the Download Accessibility Insights page.

   ![](../media/aut12.png)

1. Select the **Get** option.
   
   ![](../media/aut13.png)

1. A pop-up appears. Select the **Add extension** option from there. It will start downloading an extension in your web browser.

   ![](../media/aut14.png)

1.  Click on the **Extensions** **(1)** icon in the browser toolbar. From Accessibility Insights for Web, select the **(...)** **(2)** option and click on **Manage extension** **(3)**.
   
    ![](../media/aut15.png)

1. In the **Manage Extension** page, scroll down and click on the **Allow access to file URLs** checkbox.

   ![](../media/aut16.png)

## Task 2: Verify the GitHub Copilot Chat extension and Clone Accessible University GitHub Repo in VS Code

1. Start **Visual Studio Code** from the desktop.

    ![Picture1](../media/vscode1.jpg)

1. To verify the **GitHub Copilot Chat extension**, the following steps are to be performed within Visual Studio Code:
    - Click on the **Extensions (1)** icon in the activity bar present on the left side of the Visual Studio Code Window.
    - In the **"Search Extensions in Marketplace"** search box, type and search for the **GitHub Copilot Chat (2)** extension.
    - Select **GitHub Copilot Chat (3)** from the list of results that show up, and verify that **GitHub Copilot Chat** has been installed.
    - If not, click on the **Install (4)** button.

   ![](../media/ghc-chat-extension.png)

1. Once the installation is complete, in the left navigation pane, you will be able to see the icon for GitHub Copilot Chat, as shown below.

   ![](../media/git-chat-icon.png)

1. Skip to step 8. If you have already signed in to a GitHub Account in VS Code. If not, then follow steps 5 to 7.

1. Select the **Account** icon from bottom and click on **Sign in with GitHub**.

    ![Picture1](../media/clonerepo3.png)

1. Sign in with GitHub Credentials, and on the **Authorize GitHub for VS Code** page, click on the **Authorize Visual-Studio-Code.**

    ![Picture1](../media/clonerepo4.png)

1. If you get the pop-up, the site is trying to open the Visual Studio Code, then click on **Open**. It will navigate back to the **Visual Studio**.

    ![Picture1](../media/clonerepo5.png)

1. In the **Visual Studio Code terminal,** click on **(...)** **(1)** to select the **Terminal** **(2)** menu, followed by selecting **New Terminal** **(3)**. The terminal window usually opens in the lower half of your screen.

    ![Picture1](../media/terminal.png)
    
1. Run the following command given below to clone the Accessible University GitHub repo.

    ```
   git clone https://github.com/CloudLabsAI-Azure/AU.git
    ```

    ![Picture1](../media/clone.png)

1. Switch to the **Explorer** in the upper left corner, select **Open Folder**, and select the folder you have cloned.
   
   ![](../media/clonerepo1.png)

1. Select **Yes, I trust the authors**.

   ![](../media/clonerepo2.png)

1. Once the folder is opened, select the `before.html` file.

1. Navigate to **File Explorer** and open the folder you have cloned. From there, double-click on the `before.html` file. It will open in your web browser, where you have already added **Accessibility Insights for Web** extension.

   ![](../media/before.png)

   ![](../media/before1.png)

1. Now click on the **Extensions** button from the browser toolbar, select **Accessibility Insights for Web**, and then click on **FastPass**. It will open in a new window pop-up.

   - **FastPass**: [FastPass](https://accessibilityinsights.io/docs/web/getstarted/fastpass/) is a lightweight, two-step process that helps developers identify common, high-impact accessibility issues in less than five minutes.

   ![](../media/fastpass1.png)

   ![](../media/fastpass2.png)

1. In the new window for **Accessibility Insights for Web**, you will see the following three-step checklist for FastPass.

   - **Automated checks**: The tool automatically checks for compliance with dozens of accessibility requirements. 

   - **Tab stops**: The tool provides clear instructions, partial automation, and a visual helper that makes it easy to identify critical accessibility issues related to keyboard access, such as missing tab stops, keyboard traps, and incorrect tab order.

   - **Needs review**: The tool provides instances that need to be reviewed by a human to determine whether they pass or fail.

1. Expand the color contrast issue to check failure details.

   ![](../media/auissuedetail.png)

1. Navigate back to Visual Studio Code, Open the **before-menu.css (2)** file which is located in the **styles (1)** folder.

   ![](../media/styles1.png)

1. In the **before-menu.css** file, navigate to the CSS code for color contrast. Select the given code, press **Ctrl + i** to access the GitHub Copilot chat. Provide the given prompt and press enter.

   ```
   Fix the colour contrast issue.
   ```

   ![](../media/styles1.png)

1. Review the suggestion from GitHub Copilot, which was generated based on the context provided, ensure that it meets your requirements and Click on the **Accept** option.

   ![](../media/styles1.png)

   >**Note**: It should be noted that the code suggestions offered by GitHub Copilot might not exactly match the screenshots shown within the lab guide. GitHub Copilot is an AI-powered tool that generates code based on context and patterns, and its suggestions can be influenced by various factors.

   >**Note:** If the suggestions do not appear, consider restarting Visual Studio Code and redoing the process.

1. **Save** the file by pressing **Ctrl + S**.

1. Now refresh your **Accessible University** page. Click on the **Start over** button from the **Accessibility Insights for Web** page. You will now see a reduction in the error message.

   ![](../media/startover.png)

   ![](../media/auissuedetailreduce.png)

   >**Note**: Perform step 14 if the data wasn't reloaded.

1. Click on **html-has-lang** to review the error message.

    ![](../media/lanerror.png)

1. Navigate back to your VS Code, Open `before.html` file.

1. Select the `html` code, press **Ctrl + i** to access the GitHub Copilot chat and provide the given prompt. Click on **Enter**. 

   ```
   Add the html lang attribute.
   ```

    ![](../media/lanerror.png)

1. Review the suggestion from GitHub Copilot, which was generated based on the context provided, and ensure it meets your requirements. Click on the **Accept** option.

   ![](../media/htmlangerrorsuggestion.png)

1. After accepting the given suggestion, **save** the file by pressing **Ctrl + S**.

   ![](../media/htmlangerror.png)

1. Now refresh your **Accessible University** page. Click on the **Start over** button from  **Accessibility Insights for Web** page. You will now see a reduction in the error message.

1. Now, expand the **image-alt** to view the error message.

1. Navigate back to your VS Code.

1. In the **before-menu.css** file, Select the given code and press **Ctrl + i** to access the GitHub Copilot chat. Provide the given prompt and press enter.

   ```
   Fix the accessibility issue
   ```

1. Review the suggestion from GitHub Copilot, which was generated based on the context provided, ensure that it meets your requirements and Click on the **Accept** option.

   ![](../media/imgalterror1.png)

1. **Save** the file by pressing **Ctrl + S**.

1. Now refresh your **Accessible University** page. Click on the **Start over** button from the **Accessibility Insights for Web** page. You will now see a reduction in the error message.

   ![](../media/startover.png)

   ![](../media/auissuedetailreduce.png)

1. Now, expand the **label** to check the error message.

1. Navigate back to your VS Code.

1. In the **before-menu.css** file, Select the given code and press **Ctrl + i** to access the GitHub Copilot chat. Provide the given prompt and press enter.

   ```
   Add a label to the selected code.
   ```

   ![](../media/auissuedetailreduce.png)

1. Review the suggestion from GitHub Copilot, which was generated based on the context provided, ensure that it meets your requirements and Click on the **Accept** option.

   ![](../media/auissuedetailreduce.png) 

1. **Save** the file by **Ctrl + S**.

1. Refresh your **Accessible University** page. Click on the **Start over** button from  **Accessibility Insights for Web** page. You will now see a reduction in the error message.

1. Expand the **label** issue to check failure details.

   ![](../media/label1.png)

1. Copy the **how to fix** part, with the given **snippet** for all error and navigate back to your VS Code.

1. Click on the **GitHub Copilot Chat** window, provide the given prompt, and click on **Enter**.

   ```
   fix the label issue for
   ```

   ![](../media/label2.png)

1. **Save** the file by **Ctrl + S**.

1. Refresh your **Accessible University** page. Click on the **Start over** button from the **Accessibility Insights for Web** page. You will now see a reduction in the error message.

1. Expand the **link-in-text-block** to view the error details.

   ![](../media/linktxt.png)

1. Navigate back to your VS Code.

1. In the **before-menu.css** file, Select the given code and press **Ctrl + i** to access the GitHub Copilot chat. Provide the given prompt and press enter.

1. Review the suggestion from GitHub Copilot, which was generated based on the context provided, and ensure that it meets your requirements. click on **Enter**.

   ![](../media/linktxt3.png)

1. Change your **`before.html`** file according to the suggestions provided by GitHub Copilot.

   ![](../media/linktxt2.png)

1. **Save** the file by pressing **Ctrl + S**.

1. Refresh your **Accessible University** page. Click on the **Start over** button from the **Accessibility Insights for Web** page. You will notice that there is no issue left.

   ![](../media/allresolve.png)

### Summary

In this exercise, you successfully integrated Accessibility Insights for Web into Microsoft Edge and used it to identify accessibility issues on the AU homepage. By leveraging GitHub Copilot Chat in Visual Studio Code, you generated and implemented code solutions to fix these issues. This process ensured the website met accessibility standards, enhancing usability and inclusivity for all users, including those with disabilities. Refer to the link for more information about [Accessible University](https://www.washington.edu/accesscomputing/AU/).
