# Challenge: Document
**Description:** Read the contents of a text document and create a report based on statistics from the Save a text document to disk based on a name and content provided by the user.

**Purpose:** This application provides experience with user input and interaction in the Console, writing files to disk, working with exceptions, and writing programs in C#/.NET.

**Requirements:**

Project Name: Document

Target Platform: Console

Programming Language: C#


This program is to display the name of the app “Document” followed by a blank line, prompt the user for the name and content for a document, save the document to the current directory, and display a message if it was successful or unsuccessful based on a specification provided. The filename of the document is the name provided by the user with “.txt” appended to it.

When the program runs:

- Display “Document” followed by a blank line.
- Prompt the user for the name of the document. The user must enter a document name.
- Prompt the user for the content that is to be in the document.
- Check to see if the document name provided by the user already ends in “.txt”, do not append “.txt” to the name to create the filename. If it already has “.txt” on the end, use it as-is.
- Save the content to a file in the current directory.
- If an exception occurs, output the exception message.
- If an exception does not occur, output “[filename] was successfully saved. The document contains [count] words.” and exit. [filename] and [count] are placeholders for the filename of the document and the number of words it contains.
- After the document is saved or fails to save, prompt the user if they want to save another document. If they do, run the program again. If not, exit the program.

Note that the requirements say the file is to be saved in the current directory. This means you can use just the file name as the path for the file. If you do that, the file will be saved in the current directory for the application. When I created the project and called it Document, a directory called Document was created that contains Document.sln and another directory called Document. The Document directory inside of the project is the current directory when the application runs and is where you will find the files that are saved.

Optional Requirements:

The following requirements are not required, but you should try to implement them if you can.

Close the stream that is opened in the finally block of a try-catch-finally. Caution: test the variable holding the reference to the stream to make sure it is not null before calling the Close method on it. Calling a method on a null reference will crash the application.

