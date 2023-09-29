# Exercise 5: Using GitHub Copilot for Code Refactoring

GitHub code refactoring refers to the process of restructuring and improving the quality of code in a GitHub repository without changing its external behavior. Code refactoring aims to enhance readability, maintainability, and performance while reducing technical debt and potential bugs. 

In this exercise, you will engage in a learning or practice activity where your primary objective will be to utilize GitHub Copilot for the purpose of code refactoring.

>**Disclaimer**: GitHub Copilot will automatically suggest an entire function body or code in gray text. Examples of what you'll most likely see in this lab, but the exact suggestion may vary.

## Task 1: Understand the code already available for you

1. To demonstrate the Github code refactor, let us take an example of a poorly written code and analyze it. The below code is written using C programming language.
    
   ```
       #include <stdio.h>
       #include <stdlib.h>

       #define MAX 100

       int sum(int arr[], int n) {
           int result = 0;
           for (int i = 0; i < n; i++) {
               result += arr[i];
           }
           return result;
       }
      
       int main() {
           int n;
           printf("Enter the number of elements (1-100): ");
           scanf("%d", &n);
      
           if (n < 1 || n > MAX) {
               printf("Invalid input. Please enter a number between 1 and 100.\n");
               return 1;
           }
      
           int* arr = (int*)malloc(n * sizeof(int));
      
           if (arr == NULL) {
               printf("Memory allocation failed.\n");
               return 1;
           }
      
           printf("Enter %d integers:\n", n);
           for (int i = 0; i < n; i++) {
               scanf("%d", &arr[i]);
           }
       
           int total = sum(arr, n);
      
           printf("Sum of the numbers: %d\n", total);
      
           free(arr);
          
           return 0;
       }
    ```

1. This code is a poorly written example of a program that prompts the user for the number of elements to be summed and takes those integers as input. It employs dynamic memory allocation for the integer array and handles allocation failures with an error message. Here are some issues with the code:
    - The sum function could be renamed to something more descriptive, such as calculate_sum.
    - The scanf function calls could be wrapped in a separate function that handles the error checking and retries the input if it is invalid.
    - The error messages could be moved to a separate function that takes a message string as an argument and prints it to the console.
    - The malloc and free calls could be wrapped in a separate function that handles the error checking and frees the memory automatically when it goes out of scope.
    - The if statement that checks if the memory allocation was successful could be replaced with a call to calloc, which initializes the memory to zero and returns NULL if the allocation fails.
  
## Task 2: Use GitHub Copilot to refactor the code

1. Now, let's use the **Github Copilot Chat** feature to refactor the code.

1. Click on the **Chat** extension icon from the activity bar in the left navigation pane. This opens the GitHub Copilot Chat window into which the above code is to be pasted.

1. Give the prompt "Refactor the code" and then press **enter**.

1. The Github Copilot Chat will give the response as shown below.  

   ![Picture1](../media/refactorexamp.png)

## Task 3: Review the refactored code and understand how it works 

1. The newly generated code will look like as shown below:

     ```
        #include <stdio.h>
        #include <stdlib.h>
        
        #define MAX_ELEMENTS 100
        
        int calculate_sum(int arr[], int n) {
            int result = 0;
            for (int i = 0; i < n; i++) {
                result += arr[i];
            }
            return result;
        }
        
        int read_int(const char* prompt) {
            int value;
            do {
                printf("%s", prompt);
            } while (scanf("%d", &value) != 1);
            return value;
        }
        
        void print_error(const char* message) {
            printf("Error: %s\n", message);
        }
        
        int* allocate_int_array(int n) {
            int* arr = calloc(n, sizeof(int));
            if (arr == NULL) {
                print_error("Memory allocation failed");
                exit(1);
            }
            return arr;
        }
        
        int main() {
            int n = read_int("Enter the number of elements (1-100): ");
            if (n < 1 || n > MAX_ELEMENTS) {
                print_error("Invalid input. Please enter a number between 1 and 100.");
                exit(1);
            }
        
            int* arr = allocate_int_array(n);
        
            for (int i = 0; i < n; i++) {
                arr[i] = read_int("Enter an integer: ");
            }
        
            int total = calculate_sum(arr, n);
        
            printf("Sum of the numbers: %d\n", total);
        
            free(arr);
        
            return 0;
        }
     ```

1. Now, let's analyze the changes made by the GitHub Copilot chat. The changes made to the code by Github Copilot Chat are:
   - The MAX constant was renamed to MAX_ELEMENTS to better reflect its purpose.
   - The sum function was renamed to calculate_sum to better reflect its purpose.
   - The scanf function calls were wrapped in a separate function called read_int that handles error checking and retries the input if it is invalid.
   - The error messages were moved to a separate function called print_error that takes a message string as an argument and prints it to the console.
   - The malloc and free calls were wrapped in a separate function called allocate_int_array that handles error checking and frees the memory automatically when it goes out of scope.
   - The if statement that checks if the memory allocation was successful was replaced with a call to calloc, which initializes the memory to zero and returns NULL if the allocation fails.

1. Notice that now the code is more modular, readable, and easier to understand.

   >**Note**:It's essential to carefully review copilot suggestions before applying them.

## Task 4: Use GitHub Copilot Chat with code to refactor the code 

1. Now let us demonstrate the chat with code feature of GitHub copilot.

1. With this feature, developers can engage in real-time conversations with Copilot directly through code comments, making it feel like they are collaborating with a coding partner.

1. In the Visual Studio Code click on **Open Folder** and navigate to **C:\CloudLabs** and select the **Cloudlabs** folder.

    ![Picture1](../media/newfilecr1.png)

1. Ensure to click on **Yes, I trust the authors** within the pop-up to successfully import Cloudlabs folder into VS Code.

   ![Picture1](../media/trust-authors.png)
  
1. Now, from the File menu click on **New File** to create a new file named **chat.c**

   ![Picture1](../media/anewfilereplace.png) 

1. Paste the code given below in the newly created file.

    ```
    #include <stdio.h>
    #include <stdlib.h>
    
    int main() {
        int health = 100;
        int score = 0;
    
        printf("Welcome to the Adventure Game!\n");
        printf("You are in a dark forest.\n");
    
        while (health > 0) {
            printf("\nOptions:\n");
            printf("1. Go deeper into the forest.\n");
            printf("2. Rest by the campfire.\n");
            printf("3. Quit the game.\n");
    
            int choice;
            printf("Enter your choice: ");
            scanf("%d", &choice);
    
            switch (choice) {
                case 1:
                    printf("You venture deeper into the forest and find a treasure chest!\n");
                    score += 10;
                    break;
                case 2:
                    printf("You rest by the campfire and regain 20 health.\n");
                    health += 20;
                    break;
                case 3:
                    printf("Thanks for playing! Your score: %d\n", score);
                    exit(0);
                default:
                    printf("Invalid choice. Try again.\n");
                    break;
            }
    
            health -= 10;
            if (health <= 0) {
                printf("Game over. Your score: %d\n", score);
            }
        }
    
        return 0;
    }
     ```
1. Let's ask Copilot to use if else statements instead of the switch statement.

1. Identify the section of code where the switch statement is present and select it.

   ![Picture1](../media/selectswitch.png) 

1. Right-click on the code window and click on the **Copilot (1)** option. From the following list of options in Copilot select **Start Code Chat (2)**.
 
   ![Picture1](../media/refactorsv.png)  

1. Now type the prompt "Use if-else statements instead of the switch statement" to make the code more understandable. Copilot will give a response and you can review it and either **Accept** or **Discard** the suggestion as depicted in the image below.

   ![Picture1](../media/ifelse.png)

   >**Note:** GitHub Copilot can sometimes offer incorrect answers, so it's essential to carefully review its suggestions before applying them.

1. Save the **chat.c** file by using the **CTRL+S** keys.

## Summary

In this exercise, you have successfully employed GitHub Copilot to carry out code refactoring tasks. Code refactoring with Copilot's assistance will helps your coding projects more efficient and collaborative.
