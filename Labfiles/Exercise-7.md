# Exercise 7: Using GitHub Copilot for T-SQL and YAML code [Optional]

Duration: 20 minutes

In this exercise, the primary objective is to leverage the capabilities of GitHub Copilot, a powerful AI-assisted coding tool, to assist you in generating code for two distinct programming languages: T-SQL and YAML. You can leverage comments to generate Copilot suggestions!

>**Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in grayed text. Examples of what you'll most likely see in this exercise, but the exact suggestion may vary.

### Task 1: Generate SQL Query with GitHub Copilot using comments

1. Navigate back to Visual Studio Code and from inside the codespace in the VS Code explorer window, create a New File.

    ![](../media/chat-code-new.png)

1. Name the file `demo.sql` and type the below comment:

   ```
   -- create table for 5 products with product name and price
   ```

1. To open a new tab with multiple synthesized solutions, press `Ctrl + Enter`. GitHub Copilot will synthesize around 10 different code suggestions in a new tab. You can view the solutions and to accept a suggestion, you need to click on Accept Solution above the suggestion and then save the file.

   ![](../media/demo-sql.png)

1. After accepting the suggestion, review it carefully before applying them.

   ![](../media/demo-sql-1.png)

   >**Note**: You may not see the same suggestions as shown in the screenshot, exact suggestion may vary.

### Task 2: Generate YAML with GitHub Copilot using comments
   
1. From inside the codespace in the VS Code explorer window, create a new file.

    ![](../media/chat-code-new.png)

1. Name the file `deploy-app.yml` and type the below comment:

   ```
   # create a GitHub Action to email a report from a file at 6am daily
   ```

1. To open a new tab with multiple synthesized solutions, press `Ctrl + Enter`. GitHub Copilot will synthesize around 10 different code suggestions in a new tab. You can view the solutions and to accept a suggestion, you need to click on Accept Solution above the suggestion and then save the file.

   ![](../media/demo-yaml.png)

1. After accepting the suggestion, review it carefully before applying them.

   ![](../media/demo-yaml-1.png)

   >**Note**: You may not see the same suggestions as shown in the screenshot, exact suggestion may vary.

### Task 3: Push code to your repository from the codespace

1. Use the VS Code terminal to add files to the repository. Open VS Code Terminal if it's not opened yet.

1. Run the below command to add all the files to the repository:
   
   ```
   git add --all
   ```

1. Next from the VS Code terminal stage and commit the changes to the repository:

   ```
   git commit -m "Copilot fouth commit"
   ```

1. Finally from the VS Code terminal push to code to the repository:

   ```
   git push
   ```

   ![](../media/ex-6-push.png)

   >**Note**: Wait about 60 seconds then refresh your repository landing page for the next step.

1. You can verify the new added files available in your GitHub repository.

   ![](../media/ex-6-github.png)

### Summary

In this exercise, you have successfully generated code for SQL and YAML using comments with the help of GitHub Copilot.
