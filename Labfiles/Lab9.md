# Exercise 9: Using GitHub Copilot Workspace and File Reference

>**Note:** The results produced by **GitHub Copilot** for this particular task may not precisely align with your outcomes. This discrepancy occurs because **Github Copilot** is an AI-driven tool that can yield variable outputs from time to time.

### Task 1: Utilizing the GitHub Copilot Workspace

In this task, you will be utilizing the GitHub Copilot Workspace to enhance coding efficiency by providing contextually relevant code suggestions.

1. Open your project in VS Code, where you are signed in using the CloudLabs provided GithHub account details.

    ![](../../media/vscode-launch.png)

1. From the left pane, select the **Chat** icon. You will be provided with the **GitHub Copilot** welcome chat window.

    ![](../../media/file1.png)

1. In the textbox, enter **@** and select **Workspace** to start working with the **GitHub Copilot Workspace** agent.

    ![](../../media/file2.png)

1. Now, you can provide your own prompts and select **Submit** to get the response. To start with, you can ask **GitHub Copilot Chat** how to start your current project by providing this prompt: `How do I start the current project?`. As you submit your prompt, Copilot will automatically analyze the current workspace files and directories, split into chunks of steps:

    1. Scans the file or directory names to understand which of them are potentially relevant to providing a response.

    1. Reads file contents. Sometimes the whole file, sometimes only parts of them (due to the token memory limits).

    1. Creates context from everything it was able to collect.

    1. Starts responding, combining the context from the prompt with the one it was able to gain.

    ![](../../media/file3.png)

1. The **GitHub Copilot** would provide you with a step-by-step explanation of how to run your project. You can follow the same steps and verify that your project is running successfully.

    ![](../../media/file4.png)

1. Besides that, you can also run the command `Tell me the current workspace structure.` without the help of the **Workspace agent**, and compare the outputs.

    ![](../../media/file5.png)

    The output provided is extremely abstract, and in the end, it tells you it can't provide you with the exact solution and generates only a generic solution.

1. After this, you can try the prompt using the **Workspace** feature and get complete information about your current working project by providing the following prompt: `@workspace Tell me about the current workspace structure.`

    ![](../../media/file6.png)

    Analyze the generated output and verify that the structure is aligned with your actual project structure.

1. You can also try out the following example prompts, provide your own prompts as well as per your curiosity and requirements, and verify the output:

    ```
    @workspace Create a new lazy-loaded page with the path “/faq.”
    ```
    ```
    @workspace How can I add a new route to my ASP.NET MVC application?
    ```
    ```
    @workspace How can I handle form submissions in ASP.NET MVC?
    ```

### Task 2: Utilizing the GitHub Copilot Workspace to Create a New Application Workspace

The Github Copilot Workspace can not only provide the instructions, answers, or detailed code snippets regarding the queries you submit to it, but it can also create the complete workspace of an application from scratch. Here, you will be creating a new simple React app named **Expense Tracker** to track the expenses of the users and also modify (edit) or delete them, all with the help of the **GitHub Copilot Workspace**. You will be debugging the app using this feature itself and verifying that the app runs successfully in your local environment. To create the `Expense Tracker` app using the **GitHub Copilot workspace**, follow the below steps:

1. Open a new window in the **VS code** by choosing **File** from the topmost bar and then selecting **New Window**.

    ![](../../media/file7.png)

1. Now, select **Open Folder** from the **Welcome** page, browse to the DemoApp folder, and double-click to open it in your VS Code.

    ![](../../media/file8.png)

1. From the left pane, select the **Chat** icon. You will be provided with the **Github Copilot** welcome chat window.

    ![](../../media/file9.png)

1. In the textbox, enter **@** and select **Workspace** to start working with the **Github Copilot Workspace** agent.

    ![](../../media/file10.png)

1. Provide the prompt, `@workspace Create a workspace for the Expense Tracker application with all the necessary files and code.` In the test box, select **Submit** to generate the complete workspace of your Expense Tracker application, along with a couple of component files.

    ![](../../media/file11.png)

    >**Note:** The currrent version of **Github Copilot Workspace** allows you to create the workspace automatically with all the file structure, just click on **Create Workspace**.

1. Now, create the workspace for your **Expense Tracker** application by creating the required files and folders. To do so, select **Explorer** from the left pane, and choose the appropriate file or folder icons to create a new file or folder as per the workspace structure of your application.

    ![](../../media/file12.png)

1. The workspace structure for your **Expense Tracker** application would look similar to this, as per the output generated by the **GitHub Copilot Workspace**:

    ![](../../media/file13.png)

1. Now, generate the code for all the required components of your application by providing the relevant prompts to the **GitHub Copilot** under the **Chat** section. For instance, to create code for the **ExpenseForm.js** component of your application, write `@workspace. How can I add functionality to the ExpenseForm component to handle user input and save expenses?` and select **Submit**.

    The **GitHub Copilot** will provide you with the related code for the referenced component.

    ![](../../media/file14.png)

1. Select the **Copy** icon to copy the code and paste it into the related **ExpenseForm.js** component. Save the file.

    ![](../../media/file15.png)

    >**Note:** Read the output generated by the **Copilot** properly and make sure you install all the required packages if asked by the Copilot, before running your application.

1. Do the same for all the required components of your applications suggested by the **GitHub Copilot Workspace** in the **GitHub Copilot Chat**, and complete all the components.

1. Make sure to utilize the **GitHub Copilot Workspace** in case of any errors in any of the components of your application. Let's say an issue appears in the **app.js** file of your application. Then you can provide a similar prompt as given to know the reason behind the error and use the advanced capabilities of the **GitHub Copilot Workspace** to rectify the error: `@workspace. Fix the issue in the app.js file.`

    >**Note:** Make sure you use the **@workspace** command in the chatbox to utilize the workspace feature so that it can analyze the whole workspace files and directories of your application and provide you with the best resolution for the error that doesn't conflict with any other component.

1. You will get an output similar to this:

    ![](../../media/file16.png)

    Go through the response and resolve the errors using the steps provided in it.

1. Now, when all the errors have been fixed, you can ask Copilot how to run your application by prompting `@workspace. How can I run this app?` and submitting it.

    Follow the steps provided by it and run your application.

    ![](../../media/file17.png)

1. You can also check if all the pre-requisites required to run your **Expense Tracker** app are already in place by providing the Copilot with the prompt `@workspace. What are the prerequisites I should install to run this app?`

    ![](../../media/file18.png)

    Closely review the response generated by the **GitHub Copilot** using its workspace feature and make sure that all these prerequisites are installed. If not, install them using the steps mentioned in your answer.

1. Run the application, and it will open in your **Edge** browser as below:

    ![](../../media/file19.png)

### Task 3: Utilize the Capabilities of File Referencing

**File Referencing in GitHub Copilot** refers to the AI's ability to understand and interpret the context of your project by considering the information in other files within your workspace.

When you're working on a specific file in your codebase, **GitHub Copilot** can take into account the information, functions, classes, or variables defined in other files of your project. This means it doesn't just provide suggestions based on the current file you're working on; it can also reference other files to give you more accurate and relevant code completions. This feature is particularly useful when you're working on large projects where code is spread across multiple files. **GitHub Copilot's** ability to reference other files allows it to better understand the bigger picture of your project, resulting in more context-aware suggestions. This can significantly improve your coding efficiency and the overall quality of your code.

In this task, you will be utilizing the **GitHub Copilot File Referencing** capability to enhance coding efficiency by providing contextually relevant code suggestions. To use the File Referencing feature, follow the below steps:

1. Open your Expense Tracker project in **VS Code**, where you are signed in using the CloudLabs provided Github account details.

    ![](../../media/vscode-launch.png)

1. From the left pane, select the **Chat** icon. You will be provided with the **GitHub Copilot** welcome chat window.

    ![](../../media/file20.png)

1. In the textbox, enter **@** and select **Workspace** to activate the **GitHub Copilot Workspace** agent. You need this agent to analyze your whole workspace so that it can provide accurate answers and the related code blocks by referencing the correct files.

    ![](../../media/file21.png)

1. Now, you can use the following prompt to understand how the file referencing feature works in **GitHub Copilot**. It can accurately provide the answer for the file to which you refer: `What is the purpose of the index.js file in my project?`

    The **GitHub Copilot** will make reference to the information, functions, classes, or variables defined in the file you asked the question about and will provide you with a detailed explanation of what is in the **index.js**. Not just the explanation; it will also provide you with the related code accompanied by the answer, referenced in the provided file.

    The **GitHub Copilot** also automatically references the additional files in your project that may be required to provide you with the best answer. To get information about those files, select **Used n references** (where **n** is the total number of files referenced from your current project) present at the start of the answer and see all the files that **GitHub Copilot** referenced to provide you with the answer.

    ![](../../media/file22.png)

    Some more prompts that you can provide to understand the feature of file referencing are:

    ```
    @workspace What does the ExpenseList.js file do in my application?
    ```
    ```
    @workspace What is the purpose of the app.js file in my project?
    ```
    ```
    @workspace How can I change the CSS for my application?
    ```
    
#### **Adding a new feature in the application using File Reference:**

In this task, you will be utilizing the file reference capability to integrate a new feature in your **Expense Tracker** application. You will include a **Date** field in the **ExpenseForm** document and display it in **ExpenseItem**, and then you, will be able to sort the expenses by date in the **ExpenseList** component.

To do so, follow the below steps:

1. Open your project in VS Code, where you are signed in using the CloudLabs provided Github account details.

    ![](../../media/vscode-launch.png)

1. From the left pane, select the **Chat** icon. You will be provided with the **GitHub Copilot** welcome chat window.

    ![](../../media/file23.png)

1. In the textbox, enter **@** and select **Workspace** to activate the **GitHub Copilot Workspace** agent. You need this agent to analyze your whole workspace so that it can provide accurate answers and the related code blocks by referencing the correct files.

    ![](../../media/file24.png)

1. Now, provide this prompt to include a new **Data** field in the components and let users sort their expenses accordingly: `How can I modify the ExpenseForm component to include a date field, display this date in the ExpenseItem component, and sort the expenses by date in the ExpenseList component?`

1. The **GitHub Copilot**  feature will reference the files you asked for in the prompts as well as analyze your whole workspace and provide you with the best possible answer. It will provide you with the code snippets that you can add to the **ExpenseForm**, **ExpenseItem**, and **ExpenseList** components accordingly. You can also view the files it referenced while providing you with the answer by selecting **Used n references** (where n is the number of files referred) present at the start of the response.

    ![](../../media/file25.png)

1. You can go through the response, make the changes suggested by the **GitHub Copilot** using its file referencing feature, and edit the components as provided in the answer.

1. Run the app and verify the **Date** component is added and working properly.

    ![](../../media/file26.png)
