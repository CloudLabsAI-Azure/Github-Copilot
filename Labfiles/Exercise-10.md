# Exercise 10: Getting Started with GitHub Copilot Labs [Optional]

Duration: 20 minutes

GitHub Copilot Labs is a companion extension to GitHub Copilot that houses experimental and up-and-coming features in a sidebar.

Copilot Labs is a place for GitHub to experiment with new ideas before we take them into production. These experiments may never become part of the official product, or may change significantly before they become part of the supported product. Because they are experimental, features may break, not work as expected, or otherwise fail to meet our quality standards for production-ready code. All Copilot Labs features are provided "as-is" with no guarantees of support.

>**Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in gray text. Following are some examples of what you'll likely encounter in this lab, though the specific suggestions may differ:

## Task 1: Download Copilot Labs from the VS Code Extensions Marketplace

### Installing GitHub Copilot Labs extension in VS Code

1. To install the GitHub Copilot Labs extension, the following steps are to be performed within Visual Studio Code:
    - Click on the **Extensions** **(1)** icon in the activity bar present on the left side of the Visual Studio Code Window.
    - In the "Search Extensions in Marketplace" search box, type and search for the **GitHub Copilot Labs** **(2)** extension.
    - Select **GitHub Copilot Labs** **(3)** from the list of results that show up.
    - Click on the **Install** **(4)** button.

   ![](../media/copilot-labs-install.png)

1. As soon as you install the extension, you will see a prompt to sign in.

   ![](../media/ex10-github-signin.png)

1. When you click the 'Sign In' button in the browser window, it should open GitHub's authentication page, requesting your authorization. Click Continue.  

1. A pop-up for 'Open Visual Studio Code.app' will now appear. Click on it to proceed.

   ![](../media/ex10-allow.png)

1. Back on VS Code, a pop-up will appear asking to allow the Copilot Extension to open the URI. Click open to continue.

   ![](../media/ex10-open.png)

1. Close or exit VS Code, then run VS Code again.

1. Now click on the icon marked in red to open the Copilot Labs Section.

   ![](../media/ex10-copilot-labs.png)

## Task 2: Working with Copilot Tools

1. Code Explanation- This tool explains the code. To use this feature, **select the code** for which you want an explanation and navigate to the tools section, then click **Ask Copilot**.

   ![](../media/ex10-ask-copilot.png)

1. Once you click Ask Copilot, you will find the explanation of the code below.

   ![](../media/ex10-code-result.png)

1. Rectifying any error or bugs (Fix Bug)- This tool automatically rectifies the bug or error in the code provided. To use the code, you need to select the code to check and then 
   click on 'Fix Bug' present inside the 'Brushes' section.

   ![](../media/ex10-fixbug.png)

1. Here’s an example of how this works: In the first image, the wrong library was imported and after using the "Fix bug" feature, you can see that the issue is resolved.
   
   ![](../media/ex10-debug1.png)

   ![](../media/ex10-debug2.png)

1. In the next step, you have the debugging tool. This tool is primarily used if there are any issues in the code or if you want to add some breakpoints. Using break points, you can understand the output and flow of the code by looking at the print statements after each function.

   ![](../media/ex10-debug.png)

1. After using the debug tool, here’s the output of the code.

   ![](../media/ex10-debug-output.png)

1. A tool like this is important if you are trying to work on different matrixes or if you want to visualize the code. This code generally provides a visual output for better understanding. To start with this, you need to select the code and use the tool.

   ![](../media/ex10-debug3.png)

1. The resulting output is represented as shown below.

   ![](../media/ex10-debug4.png)

### Summary

In this exercise, you have worked on GitHub Copilot Labs and its related features.
   
