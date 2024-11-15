# Exercise 3: Exploring Python with GitHub Copilot: Intelligent Code Suggestions

### Estimated Duration: 30 minutes

GitHub Copilot accelerates the creation of programming language scripts through AI-driven code generation and intelligent tools. By analyzing context and comments, Copilot swiftly generates foundational code and offers dynamic suggestions for enhancements and optimizations.Beyond code generation, Copilot offers advanced features like autocompletion, code expansion, and suggestions for enhancing existing code or introducing new functionalities. 

>**Disclaimer**: A whole function body will be automatically suggested by GitHub Copilot in gray text. Here's an example of what you are likely to see; however, the precise recommendation could vary.

## Lab objectives

In this lab, you will complete the following tasks:

- Task 1:  Develop a Python Script for Implementing a Calculator
- Task 2: Explore GitHub Copilot Tools

## Task 1:  Develop a Python Script for Implementing a Calculator

1. From the VS Code Explorer window, create a New File.

   ![](../media/py10.png)

1. Name the file `code.py` and verify your new file looks as shown below:

   ![](../media/py1.png)

1. Now press `Ctrl + I` to open the GitHub Copilot Chat and paste the following **comments (1)** and click > or press **Enter (2)**. Copilot will give a response, and you can review it and click **Accept (3)**. Also, you can **Discard** the suggestion as depicted in the image below.
   
   ```
   Create a simple calculator that can add, subtract, multiply or divide depending upon the input from the user.
   ```

   ![](../media/py2.png)

1. Press `CTRL + S` to save the file.

1. Click on the **ellipsis (1)** on the top, click on **Terminal (2)** and select **New Terminal (3)**.

   ![](../media/openterminal.png)

1. Run the application with the **python code.py** command in the terminal and verify the output has been generated.

   ![](../media/py3.png)   

## Task 2: Explore GitHub Copilot Tools

By leveraging the previously generated code, you will explore specific tools provided by Copilot that simplifies major tasks.

1. Press `CTRL + A` to select the entire code.

1. Right click on the selected code, select **Copilot (1)** and select **Start in Editor (2)**.

      ![](../media/py11.png)

1. The following window prompts you to suggest any improvements or enhancements you would like to make to the code. Paste the following **comments (1)** and click > or press **Enter (2)**. Copilot will give a response, and you can review it and click **Accept (3)**. Also, you can **Discard** the suggestion as depicted in the image below.

   ```
   Include calculation of percentages
   ```
   
   ![](../media/py4.png)

1. Press `CTRL + S` to save the file.

1. Click on the **ellipsis (1)** on the top, click on **Terminal (2)** and select **New Terminal (3)**.

      ![](../media/openterminal.png)
   
1. Run the application with the **python code.py** command in the terminal and verify the output has been generated.

      ![](../media/py5.png)

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Explan This (2)**.

   ![](../media/py12.png)

1. It opens the GitHub Copilot Chat on the left, offering a comprehensive explanation of the code as show below.

      ![](../media/py6.png)

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Fix This (2)**.

   ![](../media/py13.png)

1. GitHub Copilot will automatically utilize the `/fix` comment to propose potential improvements to specific parts of code for enhancement. Click on **Accept** to utilize the fixes in your code.

      ![](../media/py7.png)

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Generate Docs (2)**.

      ![](../media/py14.png)

1. GitHub Copilot will automatically use the `/doc` comment to provide a breakdown of a specific line of code. Click on Accept to gain a deeper understanding while reviewing the code.

      ![](../media/py8.png)

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Generate Tests(2)**.

      ![](../media/py15.png)

1. GitHub Copilot will automatically use the `/tests` comment and open a new tab named **REFACTOR REVIEW** and will suggest the tests that can be run to verify the output.

      ![](../media/py9.png)

1. Click on **Apply**.

1. It will open a new file named **test_code.py**, displaying the test cases.

      ![](../media/py20.png)

## Review
In this lab, you learned to create a Python script for a calculator and explored GitHub Copilot tools, which streamline tasks effectively.
  
## You have successfully completed the lab
