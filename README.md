<h1>Import and parse a text file</h1>

<h2>Introduction</h2>

Security logs are often stored in text files. To analyze the security logs in these files, security analysts have to import and parse these files. Python has some functions that come in handy for these tasks, allowing analysts to efficiently access information from text files.

In this lab, you'll practice using functions and other syntax in Python to import and parse text files.

<h2>Scenario</h2>

In this lab, you're working as a security analyst. You're responsible for preparing a security log file for analysis and creating a text file with IP addresses that are allowed to access restricted information.

<h3>Task 1</h3>

In this task, you'll import a security log text file and store it as a string to prepare it for analysis.

In Python, a with statement is often used in file handling to open a file and then automatically close the file after reading it.

You're given a variable named import_file that contains the name of the log file that you want to import. Start by writing the first line of the with statement in the following code cell. Use the open() function, setting the second parameter to "r". Note that running this code will produce an error because it will only contain the first line of the with statement; you'll complete this with statement in the task after this. Be sure to replace the ### YOUR CODE HERE ### with your own code.

<img src="https://i.imgur.com/FKkoAEG.png" height="80%" width="80%"/>

<h3>Task 2</h3>

Now, you'll use the .read() method to read the imported file, and you'll store the result in a variable named text. Afterwards, display the text and explore what it contains by running the cell. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/M7Z9rFN.png" height="80%" width="80%"/>

<h3>Task 3</h3>

The output in the previous step is one big string. In this task, you'll explore how you can split the string that contains the entire imported log file into a list of strings, one string per line.

Use the .split() method to perform this split and then display the result. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

Note that displaying .split() doesn’t change what is stored in the text variable. Variable reassignment would be necessary if you want to store the result after splitting.

<img src="https://i.imgur.com/u3ukyju.png" height="80%" width="80%"/>

<h3>Task 4</h3>

There is a missing entry in the log file. You'll need to account for that by appending it to the log file. You're given the missing entry stored in a variable named missing_entry.

Use the .write() method and the parameter "a" in the open() function. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

After the portion of the code that writes to the file, another with statement uses the .read() method to read the updated file into the text variable and then display it.

<img src="https://i.imgur.com/8W1PK9p.png" height="80%" width="80%"/>

<h3>Task 5</h3>

The next task you're responsible for is creating a text file. This text file should include a list of IP addresses that are allowed to access restricted information. Documenting this in a text file will help you communicate your findings to your security team.

Start by creating a variable named import_file that stores the name of the file, which should be "allow_list.txt".

You're also given a variable named ip_addresses that stores a string containing the IP addresses that are allowed.

Run the code to display the two variables and explore what they contain. Be sure to replace the ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/jP1aFME.png" height="80%" width="80%"/>

<h3>Task 6</h3>

Your next goal is to create a with statement in order to write the IP addresses to the text file you created in the previous step.

You'll first open the file using the "w" parameter. Then, you'll write the IP addresses to the file. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell. Note that the code cell will contain a with statement that writes to a file but does not display information to the screen, so running it will not produce an output.

<img src="https://i.imgur.com/EWFjyEu.png" height="80%" width="80%"/>

<h3>Task 7</h3>

In this final step, you'll complete the code you've been writing up to this point. You'll add code to read the file containing IP addresses.

Complete a with statement that reads the text file and stores it in a new variable called text.

Afterwards, display the contents of text and run the cell to explore the result. Be sure to replace each ### YOUR CODE HERE ### with your own code before you run the following cell.

<img src="https://i.imgur.com/DKiQCbF.png" height="80%" width="80%"/>
