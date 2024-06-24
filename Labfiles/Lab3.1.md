# Lab 3.1: Best practices to use GitHub Copilot

>**Disclaimer**: A whole function body will be automatically suggested by GitHub Copilot in gray text. Here's an example of what you are likely to see; however, the precise recommendation could vary.

## Task 1:  Develop a Python Script for Implementing a Calculator

1. From the VS Code Explorer window, create a New File.

   ![](../media/.png)

1. Name the file `code.py` and verify your new file looks as shown below:

   ![](../media/.png)

1. Now press `Ctrl + I` to open the GitHub Copilot Chat and paste the following **comments (1)** and click > or press **Enter (2)**. Copilot will give a response, and you can review it and click **Accept (3)**. Also, you can **Discard** the suggestion as depicted in the image below. 
   ```
   /*
   Create a simple calculator that can add, subtract, multiply or divide depending upon the input from the user.
   */
   ```

   ![](../media/ex2-markdown.png)

1. Press `CTRL + S` to save the file.

1. Click on the ellipsis (1) on the top, click on Terminal (2) and select New Terminal (3).

1. Run the application with the **python code.py** command in the terminal and verify the output has been generated.

## Explore GitHub Copilot Tools

By leveraging the previously generated code, you will explore specific tools provided by Copilot that simplifies major tasks.

1. Press `CTRL + A` to select the entire code.

1. Right click on the selected code, select **Copilot (1)** and select **Start in Editor (2)**.

1. The following window prompts you to suggest any improvements or enhancements you would like to make to the code. Paste the following **comments (1)** and click > or press **Enter (2)**. Copilot will give a response, and you can review it and click **Accept (3)**. Also, you can **Discard** the suggestion as depicted in the image below.

   ```
   /*
   Include calculation of percentages
   */
   ```

1. Press `CTRL + S` to save the file.

1. Click on the ellipsis (1) on the top, click on Terminal (2) and select New Terminal (3).
   
1. Run the application with the **python code.py** command in the terminal and verify the output has been generated.

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Explan This (2)**.

1. It opens the GitHub Copilot Chat on the left, offering a comprehensive explanation of the code as show below.

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Fix This (2)**.

1. GitHub Copilot will automatically utilize the `/fix` comment to propose potential improvements to specific parts of code for enhancement. Click on **Accept** to utilize the fixes in your code.

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Generate Docs (2)**.

1. GitHub Copilot will automatically use the /doc comment to provide a breakdown of a specific line of code. Click on Accept to gain a deeper understanding while reviewing the code.

1. Select the code again and right click on the selected code, select **Copilot (1)** and select **Generate Tests(2)**.

1. GitHub Copilot will automatically open a new tab named **REFACTOR REVIEW** and will suggest the tests that can be run to verify the output.

1. Click on **Apply**.

1. It will open a new file named **test_code.py**, displaying the test cases.
