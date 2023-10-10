# Exercise 9: Working with the Copilot for Machine Learning [Optional]

Working with Copilot for machine learning involves leveraging GitHub Copilot, an AI-powered code completion tool developed by GitHub in collaboration with OpenAI. Here's a quick summary of the key steps and considerations:

Installation: Ensure you have GitHub Copilot installed as an extension in your integrated development environment (IDE), such as Visual Studio Code.

GitHub Integration: Link your IDE to your GitHub account to enable seamless integration. This allows Copilot to access your code repositories and provide context-aware suggestions.

Machine Learning Frameworks: Copilot supports various machine learning libraries and frameworks like TensorFlow, PyTorch, scikit-learn, and more. It can assist with code generation for tasks like data preprocessing, model building, and evaluation.

In this exercise, you will be cloning the git repository with required dataset into your environment. Here, you will be working with Copilot for Machine learning involves leveraging GitHub Copilot.

>**Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in grayed text. Examples of what you'll most likely see in this exercise, but the exact suggestion may vary.

>**Note**: Before proceeding with the exercise, make sure you have installed Python and pip-packages.

### Task 1: Pre-requisites and Injecting the required dataset into your environment

1. Open VS Code Terminal by clicking on **Ellipsis (...)** **(1)**, select **Terminal** **(2)** and click on **New Terminal** **(3)**.

   ![](../media/ex-8-openterminal.png)

1. Clone the below git repository in your environment.

   ```
   git clone https://github.com/CloudLabsAI-Azure/ml-copilot-workshop.git
   ```

1. Change the directory in terminal by running the below command:

   ```
   cd ml-copilot-workshop
   ```

1. To install all the required python dependencies in your environment, before working with copilot run the below command in your terminal:

   ```
   pip install -r requirements.txt
   ```

### Task 2: Auto Completion of Code with different experiments

1. From the VS Code explorer window, right-click on the folder named **ml-copilot-workshop** **(1)** and click on **New File**. Name the file as `Experiments.ipynb` **(2)** and verify your new file looks as shown below:

   ![](../media/ex-8-create-file.png)

1. Type the below comments to import all the libraries the copilot automatically prompts all the libraries press tab and then press enter to get the output. 

   ```
   # import libraries with respect to loading data and creating random forest model
   ```

   ![](../media/ex-8-import-lib.png)

1. Accept all the suggestions for importing libraries as shown in the below screenshot **(1)** and click **Run** **(2)** button to execute the cell. CLick on `+ Code` **(3)** to add the new cell.

   ![](../media/ex8-add-cell-new.png)

   >**Note**: While running the cell, you may need to install the required packages and select kernel.

1. Type the below comments to load the data using copilot prompt. Press enter to get into next line and review the suggestion and press Tab to accept the suggestion.

   ```
   # load the data from csv file and the name of the file is diabetes.csv
   ```

    ![](../media/ex8-load-data-1.png)

1. Now cli k on **+Code** and move to next task.

   
### Task 3: Mathematical and machine Learning with different Examples

1. Type the below comments to Performe the data analysis and summary statistics on dataset, press tab and then press enter to get the output. 

   ```
   # Perform count, min, max, std, mean, 25%, 50%, 75% on the dataset
   ```

   ![](../media/ex9-machine-learning-dataset.png)

1. Once the cell run is completed, you will be getting the output similar to the below image.

   ![](../media/ex9-machine-learning-output.png)

1. Before building the model the main frame is to split the data into train test and split and this would be done by copilot itself. Type the below comments, press tab

     ```
   # 
   ```

   ![](../media/ex9-machine-learning-dataset.png)
