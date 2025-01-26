
# Lab 5: Code Refactoring
---
## Lab Objective 

GitHub code refactoring refers to the process of restructuring and improving the quality of code in a GitHub repository without changing its external behaviour. Code refactoring aims to enhance readability, maintainability, and performance while reducing technical debt and potential bugs. 

In this exercise, you will participate in a learning or practice activity where your main goal will be to use GitHub Copilot for code refactoring using the C# programming language. You will also be generating unit test functions using GitHub Copilot Chat.

>**Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in gray text. Examples of what you'll most likely see in this lab, but the exact suggestion may vary.

## Task 1: Understand the code already available for you.

Install the C# extension in VS Code for enhanced C# development features.

1. In the LABVM desktop search for **Microsoft Edge** **(1)**, click on **Microsoft Edge** **(2)** browser.

   ![Edge](../../media/Edge.png)

1. Navigate to GitHub login page using the provided URL below:
   [https://github.com/login](https://github.com/login)

1. On the **Sign in to GitHub** tab, you will see the login screen. In that screen, enter the **email** **(1)** and **password** **(2)**. Then click on **Sign in** **(3)**. 

   ![GitHub Login](../../media/github-login.png)

   >**Note:** To view the GitHub credentials, access the lab named **GitHub Copilot Lab: GitHub Credentials**, which is present within the First learning path of this course.

      ![GitHub Credentials](../../media/credsfile.png)

   >**Note:** Once the lab has been deployed successfully, navigate to the **Environment** tab to view the key-value pairs of the **GitHub UserEmail**, and **GitHub Password**. You can use the copy buttons under the actions column to have the values copied instantly. Alternatively, it is suggested to have the values copied over onto a notepad for easy accessibility. 

      ![GitHub Credentials in Environment](../../media/githubcreds.png)

   >**Note:** If you're unable to copy the username and password, please type them manually to proceed further.
          
1. Navigate to Outlook login page using the provided URL below:
   [https://outlook.office365.com/mail/](https://outlook.office365.com/mail/)
1. Next, to get the authentication code, sign in to Outlook with the git credentials within the Environment tab from the previous step. Once you have logged into Outlook, find the recent email containing the verification code. Enter the verification code, and click on **Verify**.

   >**Note:** The email containing the verification code can sometimes creep into the archive/spam folders within your Outlook.

   ![Outlook Authentication](../../media/authgit.png)

1. Now, right-click on your profile icon in the top right and click on **Your Repositories**.

   ![GitHub Repositories](../../media/Copilotrepo.png)

1. Click on the repository named **skills-copilot-codespaces-vscode**.

1. Navigate back to the home page of your repository by clicking the **Code** **(1)** tab located at the top left of the screen. Click the **Code** **(2)** button located in the middle of the page.

   ![Code Tab](../../media/code-code.png)

1. Click the **Codespaces (1)** tab on the box that pops up and then click the **+ (2)** button.

   ![Codespaces Tab](../../media/labgit.png)

   >**Note**: If the pop-up prompt doesn't appear in the browser to open Visual Studio code, manually launch Visual Studio code from the desktop and close it. Next, return to the browser, refresh the page, and launch the codespace that was previously created.

1. You will encounter a pop-up prompt. Click **Open** to proceed. Subsequently, another pop-up window will appear within Visual Studio Code (VS Code), where you should once again select **Install and Open** to continue.

   ![Open VS Code](../../media/open.png)

   ![VS Code Codespaces](../../media/codespaces.png)

1. At the bottom right corner, you will get a prompt to sign in to GitHub.

   ![Sign in to GitHub](../../media/signingit.png)

   >**Note:** If you do not get the sign-in prompt within Visual Studio Code, click on **Allow** in the pop-up that appears which will open a window in the browser, refresh the screen and click on **Open** in the pop-up that appears.

1. Next, once you get the popup, click on **Allow**.

   ![Allow GitHub Access](../../media/allow.png)

   >**Note**: Wait about 2 minutes for the codespace to spin itself up.

1. If a page **GitHub for VS Code is requesting additional permissions** opens then click on **Authorize Visual-Studio-Code**.

    ![Authorize Visual Studio Code](../../media/1.png)

1. Verify your codespace is running. Make sure the VS code looks as shown below:

   ![VS Code Running](../../media/lab5files.png)

1. Click on **Extensions** **(1)** from the left menu, and the **GitHub Copilot** **(2)** extension should show up in the VS Code extension list. Click the Copilot extension and verify its installation as shown below:

   ![Verify Copilot Installation](../../media/verify-copilot.png)

   >**Note**: If the GitHub Copilot extension is not installed, click on Install.

1. In the "Search Extensions in Marketplace" search box, type and search for the **GitHub Copilot Chat** extension.

1. Select **GitHub Copilot Chat** from the list of results that show up, and verify that **GitHub Copilot Chat** has been installed.

1. If not, click on the **Install** button.

    ![GitHub Copilot Chat Extension](../../media/ghc-chat-extension.png)

1. Once the installation is complete, in the left navigation pane you will be able to see the icon for GitHub Copilot Chat as shown below.

   ![GitHub Copilot Chat Icon](../../media/git-chat-icon.png)

1. In the Visual Studio Code window, to install the **C Sharp (C#)** extension, the following steps are to be performed:
    - Click on the **Extensions** **(1)** icon in the activity bar present on the left side of the Visual Studio Code Window.
    - In the "Search Extensions in Marketplace" search box, type and search for the **C#** **(2)** extension.
    - Select **C#** **(3)** from the list of results that show up.
    - Click on the **Install** **(4)** button.

      ![C# Installation](../../media/csharp-install.png)

      >**Note**: If you get a pop-up for Update Visual Studio Code, go to the **Settings (1)** icon from the left navigation pane and choose **Install update (2)** and wait until updates complete then when **Restart Visual Studio Code to apply the latest update** prompted select **Update Now (3)** and close and open Visual Studio then proceed with the above step.

      ![Update VS Code](../../media/image1.png)
   
      ![Update Visual Studio](../../media/image2.png)

      
1. Make sure to sign in to your GitHub account by clicking on the **GitHub Copilot icon** located in the bottom right corner.

    ![](../../media/githubsignin2.png)

    > **Note:** Click "**Allow**" for VS Code to sign in to your GitHub account. A new web page will open. Copy the URL of the page, paste it into a private browser, enter your GitHub credentials, and sign in.

1. To demonstrate the GitHub code refactor, let us take an example of a poorly written code and analyze it. The below code is written using the C# programming language.
    
   ```
   using System;

   class Program
   {
       const int MAX = 100;

        static int Sum(int[] arr, int n)
        {
            int result = 0;
            for (int i = 0; i < n; i++)
            {
                result += arr[i];
            }
            return result;
        }

        static void Main()
        {
            int n;
            Console.Write("Enter the number of elements (1-100): ");
            if (!int.TryParse(Console.ReadLine(), out n) || n < 1 || n > MAX)
            {
                Console.WriteLine("Invalid input. Please provide a digit ranging from 1 to 100.");
                Environment.Exit(1);
            }

            int[] arr = new int[n];

            Console.WriteLine("Enter " + n + " integers:");
            for (int i = 0; i < n; i++)
            {
                if (!int.TryParse(Console.ReadLine(), out arr[i]))
                {
                    Console.WriteLine("Invalid input. Please enter valid integers.");
                    Environment.Exit(1);
                }
            }

            int total = Sum(arr, n);

            Console.WriteLine("Sum of the numbers: " + total);

            // No need to free memory in C#, as it's managed by the runtime.
        }
    }      
   ```

1. This code is a poorly written example of a program that prompts the user for the number of elements to sum and takes those integers as input. It employs dynamic memory allocation for the integer array and handles allocation failures with an error message. Here are a few code-related issues:
    - The code begins with the inclusion of the System namespace for essential input and output operations.
    - It defines a constant MAX with a value of 100 to represent the maximum number of elements allowed.
    - The Sum method calculates the sum of elements in an array.
    - In the Main method:
      - It prompts the user to enter the number of elements (between 1 and 100) and validates the input.
      - Allocates an array 'arr' to store the entered integers.
      - Prompts the user to enter the specified number of integers and validates each input.
      - Calculates the sum of the entered integers using the Sum method.
      - Outputs the sum to the console.
      - There's no need to manually free memory in C# because it manages memory automatically.
  
## Task 2: Use GitHub Copilot to refactor the code

Use GitHub Copilot to improve and restructure code for better readability and efficiency.

1. Now, let's use the **GitHub Copilot Chat** feature to refactor the above code.

1. Click on the **Copilot** extension icon from the activity bar in the top navigation pane next to the search bar and Choose **Open Chat** option from the dropdown. This opens the GitHub Copilot Chat window into which the above code is to be **pasted**.

1. Type the prompt `Refactor the code` at the end of the code and then press **enter**.

1. The GitHub Copilot Chat will give the response as shown below.

   ![](../../media/refactored-code.png)

## Task 3: Review the refactored code and understand how it works.

Review the refactored code which more understandable and clean. 

1. The newly generated code will look as shown below:

     ```
     using System;

     class Program
     {
        const int MAX = 100;

        static int Sum(int[] arr)
        {
            int result = 0;
            foreach (int num in arr)
            {
                result += num;
            }
            return result;
        }

        static void Main()
        {
            int n;
            Console.Write("Enter the number of elements (1-100): ");
            if (!int.TryParse(Console.ReadLine(), out n) || n < 1 || n > MAX)
            {
                Console.WriteLine("Invalid input. Please enter a number between 1 and 100.");
                Environment.Exit(1);
            }

            int[] arr = new int[n];

            Console.WriteLine("Enter " + n + " integers:");
            for (int i = 0; i < n; i++)
            {
                if (!int.TryParse(Console.ReadLine(), out arr[i]))
                {
                    Console.WriteLine("Invalid input. Please enter valid integers.");
                    Environment.Exit(1);
                }
            }

            int total = Sum(arr);

            Console.WriteLine("Sum of the numbers: " + total);
        }
    }
    ```

1. Now, let's analyze the changes made to the code by GitHub Copilot Chat
   - Here, GitHub Copilot removed the `n` parameter from the Sum method since it's not needed. Instead, the Copilot used a for-each loop to iterate over the array. As a result, the code is easier to comprehend and more concise.
   - This includes the system namespace for input and output operations.
   - Defines a constant MAX with a value of 100 for the maximum number of elements allowed in an array.
   - The Sum method calculates the sum of elements in an integer array using a for-each loop.
   - In the Main method:
     - Asks the user to input the number of elements and validate it.
     - Creates an integer array to store user-entered values.
     - Prompts the user to enter integers, validates the input, and stores them in the array.
     - Calculates the sum of the integers using the Sum method.
     - Shows the sum on the console.
     - The code includes input validation and provides the sum of user-entered integers.

1. Notice that now the code is more modular, readable, and easier to understand.

   >**Note**: It's essential to carefully review copilot suggestions before applying them.

## Task 4: Use GitHub Copilot Chat with code to refactor the code 

In this task, you will demonstrate the chat with code feature of GitHub Copilot. With this feature, developers can engage in real-time conversations with Copilot directly through code comments, making it feel like they are collaborating with a coding partner.

1. From the codespace in the VS Code Explorer window, create a new file.

    ![](../../media/chat-code-new.png)

1. Name the file `codechat.cs` and if you see a recommendation to install the `C#` extension. Click on Install.

   ![](../../media/chat-code-file.png)

1. Copy and paste the code given below in the newly created file, i.e., `codechat.cs`.

    ```
    using System;

    class Program
    {
        static void Main()
        {
            int health = 100;
            int score = 0;

            Console.WriteLine("Welcome to the Adventure Game!");
            Console.WriteLine("You are in a dark forest.");

            while (health > 0)
            {
                Console.WriteLine("\nOptions:");
                Console.WriteLine("1. Go deeper into the forest.");
                Console.WriteLine("2. Rest by the campfire.");
                Console.WriteLine("3. Quit the game.");

                int choice;
                Console.Write("Enter your choice: ");
                if (int.TryParse(Console.ReadLine(), out choice))
                {
                    switch (choice)
                    {
                        case 1:
                            Console.WriteLine("You go farther into the forest and discover a treasure chest!");
                            score += 10;
                            break;
                        case 2:
                            Console.WriteLine("You rest by the campfire and regain 20 health.");
                            health += 20;
                            break;
                        case 3:
                            Console.WriteLine($"Thanks for playing! Your score: {score}");
                            return;
                        default:
                            Console.WriteLine("Invalid choice. Try again.");
                            break;
                    }

                    health -= 10;
                    if (health <= 0)
                    {
                        Console.WriteLine($"Game over. Your score: {score}");
                    }
                }
                else
                {
                    Console.WriteLine("Invalid input. Please enter a valid number.");
                }
            }
        }
    }
    ```

1. Let's ask Copilot to use if else statements instead of the switch statement.

1. Identify the section of code where the switch statement is present and select it.

1. Right-click on the code window and click on the **Copilot** option. From the following list of options in Copilot, select **Editor Inline Chat**.
 
   ![](../../media/gc3.png)  

1. Now type the prompt "Use if-else statements instead of the switch statement" **(1)** to make the code more understandable and click `>` or press `Enter` **(2)**. Copilot will give a response, and you can review it and click **Accept** **(3)**. Also, you can **Discard** the suggestion as depicted in the image below.Press `Ctrl + S` to save the file.

    ![](../../media/chat-code-accept.png)

     >**Note:** It's essential to carefully review copilot suggestions before applying them.

## Task 5: Create unit test functions

Use GitHub Copilot Chat to generate a full JavaScript program based on a provided prompt.Write automated tests to verify code functionality and correctness.

1. From the codespace in the VS Code Explorer window, create a new file.

    ![](../../media/chat-code-new.png)

1. Name the file `test.js` as shown below:  

   ![](../../media/create-test.png)

1. Now, navigate to the GitHub Copilot Chat and give the prompt **Compose a full JavaScript program for constructing a calculator**.

1. GitHub Copilot Chat will generate code based on the prompt you provide, as shown below.

   ![](../../media/calci.png)

   >**Note**: The code shown in the screenshot may be different for you.

1. Copy and paste the code in the file named **test.js** that you just created and press `Ctrl + S` to save the file..

1. Now, to generate test cases for each function, select the function for which the test case has to be generated, and back in the GitHub Copilot Chat window, type **/tests** and hit enter.

   ![](../../media/abctestsdemo.png)

1. It will generate a test case for the add function.

   ![](../../media/addtestcase.png)

### Task 6: Push code to your repository from the codespace

Commit and push the updated code to a GitHub repository for version control.

1. Use the VS Code terminal to add files to the repository. Open VS Code Terminal if it's not opened yet.

1. Run the below command to add the `codechat.cs`, `test.js`  files to the repository:

   ```
   git add codechat.cs test.js
   ```

1. Next, from the VS Code terminal stage, commit the changes to the repository:

   ```
   git commit -m "Copilot third commit"
   ```

1. Finally, from the VS Code terminal, push to code to the repository:

   ```
   git push
   ```

   ![](../../media/ex-4-push5.png)

    > **Congratulations** on completing the lab! Now, it's time to validate it. Here are the steps:
    > - On GitHub, locate your profile photo at the top right corner of the screen.
    > - Copy your GitHub username.

     ![Picture1](../../media/gihubuser15.png)
   
    > - Hit the Validate button for the corresponding task. Paste your GitHub username into the required field and click on submit.

     ![Picture1](../../media/gihubuser115.png)

   > - If you receive a success message, you can proceed to the next task.
   > - If not, carefully read the error message and retry the step, following the instructions in the lab guide. 
   > - If you need any assistance, please contact us at cloudlabs-support@spektrasystems.com. We are available 24/7 to help you out.
   
   <validation step="d30ee72a-72c4-4c44-a120-080c4ef5b834" />

## Summary

In this lab, you have successfully employed GitHub Copilot to carry out code refactoring tasks and created unit test functions. Code refactoring with Copilot's assistance will make your coding projects more efficient and collaborative.

## You have successfully completed this lab. 
