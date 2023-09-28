# Exercise 4: Using GitHub Copilot Chat to generate ARM and Terraform code with Copilot

### About GitHub Copilot Chat and Visual Studio Code

GitHub Copilot Chat is a chat interface that lets you ask and receive answers to coding-related questions directly within a supported IDE. Copilot Chat can help you with a variety of coding-related tasks, like offering you code suggestions, providing natural language descriptions of a piece of code's functionality and purpose, generating unit tests for your code, and proposing fixes for bugs in your code. For more information, see "[About GitHub Copilot Chat](https://docs.github.com/en/copilot/github-copilot-chat/about-github-copilot-chat)."

### Use cases for GitHub Copilot Chat

GitHub Copilot Chat can provide coding assistance in a variety of scenarios.

 - Generating unit test cases
 - Explaining code
 - Proposing code fixes
 - Answering coding questions

In this exercise, you will be installing GitHub Copilot Chat extension and you will be generating ARM and Terraform code with Copilot.

#### Task 1: Installing GitHub Copilot Chat extension in VS Code

1. To install the GitHub Copilot Chat extension, the following steps are to be performed within Visual Studio Code:
    - Click on the **Extensions (1)** icon in the activity bar present on the left side of the Visual Studio Code Window.
    - In the "Search Extensions in Marketplace" search box, type and search for the **GitHub Copilot Chat (2)** extension.
    - Select **GitHub Copilot Chat (3)** from the list of results that show up.
    - Click on the **Install (4)** button.

   ![](../media/ghc-chat-extension.png)

1. Once the installation is complete, in the left navigation pane you will able to see the icon for GitHub Copilot Chat as shown in the below.

   ![](../media/git-chat-icon.png)

### Task 2: Generate Code by Chat that uses ARM to deploy resources to Azure

1. In the Visual Studio Code activity bar, click the GitHub Copilot Chat icon to open the GitHub Copilot Chat chat window.

1. At the bottom of the GitHub Copilot Chat window, in the **Ask Copilot a question or type / for topics** text box, type a coding-related question, then press Enter. For example, type "Write a ARM code for deploying Storage Account to Azure."

    ![](../media/create-arm.png)

1. GitHub Copilot Chat will process your question and provide an answer, with code suggestions when appropriate, in the chat window. 

    ![](../media/arm-result.png)

    >**Note**: Optionally, if GitHub Copilot Chat suggests a follow-up question above the **Ask Copilot a question or type / for topics** text box, click the follow-up question to ask it.

    >**Note**:  If your question is outside the scope of GitHub Copilot Chat, it will tell you and may suggest an alternative question to ask.
   
1. You can view response from GitHub Copilot in the Chat and 