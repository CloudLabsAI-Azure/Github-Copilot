# Exercise 10: Working with the Copilot for Machine Learning [Optional]

### Estimated Duration: 30 minutes

Working with Copilot for machine learning involves leveraging GitHub Copilot, an AI-powered code completion tool developed by GitHub in collaboration with OpenAI. Here's a quick summary of the key steps and considerations:

Installation: Ensure you have GitHub Copilot installed as an extension in your integrated development environment (IDE), such as Visual Studio Code.

GitHub Integration: Link your IDE to your GitHub account to enable seamless integration. This allows Copilot to access your code repositories and provide context-aware suggestions.

Machine Learning Frameworks: Copilot supports various Machine Learning libraries and frameworks like TensorFlow, PyTorch, scikit-learn, and more. It can assist with code generation for tasks like data preprocessing, model building, and evaluation.

In this exercise, you will be cloning the Git repository with the required dataset into your environment. Here, you will be working with Copilot for Machine Learning, which involves leveraging GitHub Copilot.

>**Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in grayed text. Examples of what you'll most likely see in this exercise, but the exact suggestion may vary.

>**Note**: Before proceeding with the exercise, make sure you have installed Python and pip packages.

>**Note**: If you are unable to see any suggestions by GitHub Copilot in VS Code, please restart the VS Code once and try again. 

## Lab objectives

You will be able to complete the following tasks:

- Task 1: Prerequisites and Injecting the Required Dataset into Your Environment
- Task 2: Auto_Completion of Code with Different Experiments
- Task 3: Mathematical and Machine Learning with Different Examples
- Task 4: Data Visualization and Data Transformation
- Task 5: Training the sample model

### Task 1: Prerequisites and Injecting the Required Dataset into Your Environment

1. Open VS Code Terminal by clicking on **Ellipsis (...)** **(1)**, selecting **Terminal** **(2)**, and clicking on **New Terminal** **(3)**.

   ![](../media/ex-8-openterminal.png)

1. Clone the below git repository in your environment.

   ```
   git clone https://github.com/CloudLabsAI-Azure/ml-copilot-workshop.git
   ```

1. Change the directory in the terminal by running the below command:

   ```
   cd ml-copilot-workshop
   ```

1. To install all the required Python dependencies in your environment before working with Copilot run the below command in your terminal:

   ```
   pip install -r requirements.txt
   ```

### Task 2: Auto_Completion of Code with Different Experiments

   >**Note**: If the suggestion doesn't appear or if the output isn't generated as expected, press **Ctrl+I**, paste the comments, review the suggestions, and then accept them. 

1. To install the **Jupyter**, the following steps are to be performed within Visual Studio Code:
    - Click on the **Extensions (1)** icon in the activity bar present on the left side of the Visual Studio Code Window.
    - In the **"Search Extensions in Marketplace"** search box, type and search for the **Jupyter (2)** extension.
    - Select **Jupyter (3)** from the list of results that show up, and verify that **Jupyter** has been installed.
    - If not, click on the **Install in Codespaces: ubiquitous space doodle(4)** button.

   ![](../media/c37.png)

1. From the VS Code explorer window, right-click on the folder named **ml-copilot-workshop** **(1)** and click on **New File**. Name the file `Experiments.ipynb` **(2)** and verify that your new file looks as shown below:

   ![](../media/ex-8-create-file.png)

1. Click on the file, select **+ Code**.

   ![](../media/c38.png)

1. Click on **Select Kernel** from the top right, select the **Python Environment** and then choose Python **3.12**.   

1. Type the below comments to import all the libraries where the Copilot automatically prompts all the libraries; press **Enter** to get into the next line and review the suggestion, press **tab**. *Repeat this untill the Load data comment appears* and click on **Run** button to execute the cell.

   ```
   # Import libraries with respect to loading data and creating a random forest model
   ```

   ![](../media/ex-8-import-lib-1.png)

1. Accept all the suggestions for importing libraries as shown in the below screenshot **(1)** and click the **Run** **(2)** button to execute the cell. Click on `+Code` **(3)** to add the new cell.

   ![](../media/ex8-add-cell-new-1.png)

   >**Note**: While running the cell, you may need to install the required packages and select the kernel.

1. Type the below comments to load the data using the Copilot prompt. Press **Enter** to get into the next line and review the suggestion, and press **tab** to accept the suggestion **(1)** and click on **Run (2)** button to execute the cell.

   ```
   # Load the data from a csv file, and the name of the file is diabetes.csv
   ```

    ![](../media/ex8-load-data-1-2.png)

    ![](../media/c39.png)    

1. Now click on **+Code** and move on to the next task.

   
### Task 3: Mathematical and Machine Learning with Different Examples

### Task 3.1: Mathematical Operations

   >**Note**: If the suggestion doesn't appear or if the output isn't generated as expected, press **Ctrl+I**, paste the comments, review the suggestions, and then accept them. 

1. Type the below comments to perform the first mathematical experiment would be to generate the birth year from the age column present in the dataset. Press **enter** to get into the next line and review the suggestion, and press **tab** to accept the suggestion and click on **Run** button to execute the cell.

   ```
   # Mathematical operations on the dataset, like generating the birth year from age
   ```

   ![](../media/ex9-birthyear.png)

   >**Note**: If the suggestion doesn't appear, press **Ctrl+I**, paste the comments, review the suggestions, and then accept them.  
   >**Note**: Continue clicking on **+Code** after each comment till the last task of this exercise.

1. Type the below comment, Press **Enter** to get into the next line and review the suggestion, and press **tab**  twice to get the output similar to the below image and click on **Run** button to execute the cell. 

   ```
   # Show the new column
   ```

   ![](../media/c40.png)

1. Type the below comments to convert the BMI column up to two decimal values, press "tab". Press **enter** to get into the next line and review the suggestion, and press **tab** to accept the suggestion and click on **Run** button to execute the cell.

   ```
   # Convert the BMI column to two decimal values
   ```

   ![](../media/ex9-bmi-decimal.png)

1. In the same code cell, type the below comment. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to execute the cell.

   ```
   # Show the new column only
   ```

   ![](../media/ex9-bmi-decimal-output.png)


### Task 3.2: Machine Learning

   >**Note**: If the suggestion doesn't appear or if the output isn't generated as expected, press **Ctrl+I**, paste the comments, review the suggestions, and then accept them. 

1. Type the below comments to perform the data analysis and summary statistics on dataset. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to execute the cell.

   ```
   # Perform count, min, max, std, mean, 25%, 50%, and 75% on the dataset
   ```

   ![](../media/ex8-machine-learning-dataset.png)

1. Once the cell run is completed, you will get an output similar to the below image.

   ![](../media/ex8-machine-learning-output.png)

1. Before building the model, the main frame is to split the data into train tests and splits and this would be done by Copilot itself. Type the below comments. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to execute the cell.

   ```
   # Split the data into training and testing data and the column name Diabetic is the target column
   ```

   ![](../media/ex9-train-data.png)

   ![](../media/ex9-train-data-1.png)


### Task 4: Data Visualization and Data Transformation

### Task 4.1: Data Visualization

   >**Note**: If the suggestion doesn't appear or if the output isn't generated as expected, press **Ctrl+I**, paste the comments, review the suggestions, and then accept them. 

1. Click on **+Code** to open the new cell and type the below comments to perform the basic operations on dataset. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to execute the cell.

   ```
   # Perform univariate analysis on the dataset and plot the graphs.hist
   ```

      ![](../media/ghvi1.png)

1. Once the cell run is completed, you will be getting a graphical representation output similar to the below image.

      ![](../media/ghvi2.png)

1. Now, type the below comments for specifying certain commonly used plots for visualization. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to get the output as shown in the below-given image.

   ```
   # Perform scatter plot on the dataset and plot the graphs
   ```

   ![](../media/ex9-scatter-graph.png)

1. Type the below comments for performing Joint Plot or Grid (rarely used plots) for visualization. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to get the output as shown in the below-given image.

   ```
   # Perform Joint Grid plot on the dataset and plot the graphs
   ```

   ![](../media/ex9-jointgrid-graph.png)

   ![](../media/ex9-jointgrid-graph-output.png)

1. Type the below comments for performing visualization on all features of the dataset. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button to get the output as shown in the below-given image.

   ```
   # Perform comparison on all features of the dataset and plot the graphs in a single plot using heatmap
   ```

   ![](../media/ex9-heatmap.png)

   ![](../media/ex9-heatmap-output.png)


### Task 4.2: Data Transformations


1. Click **+Code** to add a new cell and type the below comments for Standardization which is the process of scaling and centering numeric features to have a mean of 0 and a standard deviation of 1, making them comparable and suitable for certain algorithms. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button

   ```
   # Perform standardization on the data
   ```

   ![](../media/ex9-standardization.png)

   ![](../media/ex9-standardization-new.png)

1. You will get the output as shown in the below-given image once the code cell finishes running.

   ![](../media/ex9-standardization-output.png)


### Task 5: Training the sample model

Training a sample model using Random Forest.

>**Note**: The model training is a continuation of the train test split step to train the model; run the train test split step first and then continue with the model building.

1. Click **+ Code** to add a new cell and type the below comments for creating the random forest model. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button

   ```
   # Create a random forest model with 100 trees, and the criterion is entropy
   ```

   ![](../media/ex9-entropy.png)

   ![](../media/ex9-entropy-1.png)

   ![](../media/ex9-entropy-2.png)

1. In a new cell type the below comments for calculating the accuracy of the model. Press **enter** to get into the next line and review the suggestion, and press **tab** twice to accept the suggestion and click on **Run** button

   ```
   # Calculate the accuracy of the model
   ```

   ![](../media/ex9-accuracy.png)


### Summary

In this exercise, you have successfully leveraged the GitHub Copilot for Machine Learning.

## You have successfully completed the lab. Click on **Next >>** to procced with next exercise.
