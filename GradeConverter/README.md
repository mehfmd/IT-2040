# Challenge: GradeConverter
**Description:** Write a program that converts number scores into the correct letter grade, e.g. 88 = "B", and 76 = "C". The program will also produce statistics for the grades.

**Purpose:** This application provides experience with user input and interaction in the Console, writing functions, using lists and loops, and writing programs in C#/.NET.

**Requirements:**

- Project Name: GradeConverter
- Target Platform: Console
- Programming Language: C#

In schools, numerical grades have a corresponding letter grade. You program will do the following:

- Ask the user to enter their first and last name
- Print a welcome message: "Hello [first name] [last name] Welcome to the Grade Converter!"
- Prompt the user to enter the number of grades they need to convert "Enter the number of grades you need to convert: "
- Prompt the user to enter the grades. The grades should be stored in a list and you should use the appropriate data type for the grades. Grades can be whole numbers like 77, or have a decimal, like 77.3. Note: Your program should not crash because of bad input.
- Convert the number grades to letter grades using the following scale: (A = 90-100, B = 80-89, C = 70-79, D = 60 - 69, F lower than 60). Note: this scale includes fractional grades so an 89.5 would be a "B".
- Print all the numerical grades and their corresponding letter grades to the console like the following example: "A score of  89.5 is a B grade"
- Print statistics for the list of grades. You should print the number of grades, and the average grade. The output should look like the following:


Grade Statistics

Number of grades: 10
Average Grade: 81, which is a B"

- Ask the user if they have more grades to convert. If they don't have more grades to convert you should end the program. If they do have more grades to convert you should run the program again.

Program Design:

You are required to write functions to do the following:

- Write a function that prompts the user to enter the number grades.
- Write a function that converts a score to its corresponding letter grade.
You should not use built-in C# functions to calculate the highest and lowest grade. You should code those yourself.
Your program should not crash for any reason. You should handle any exception(s) that may occur.
