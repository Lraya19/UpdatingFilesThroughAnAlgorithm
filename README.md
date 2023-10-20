<h1>Python - Updating Files Through a Python Algorithm</h1>


<h2>Description</h2>
Project consists of working as a security analyst. At our organization, access to restricted content is controlled with an allow list of IP addresses. The “allow_list.txt” file identifies these IP addresses. A separate remove list identifies IP addresses that should no longer have access to this content. I created an algorithm to automate updating the “allow_list.txt” file and remove these IP addresses that should no longer have access.
<br />


<h2>Languages and Utilities Used</h2>
 
- <b>Python</b>

<h2>Environments Used </h2>

- <b>Windows 11</b> (22H2)

<h2>Program walk-through:</h2>

<p align="center"> 
 <br/>We’ll import a security log text file and store it as a string to prepare it for analysis. In Python, a with statement is often used in file handling to open a file and then automatically close the file after reading it.

<p align="center">
  Task 1:
  
  We’re given a variable named import_file that contains the name of the log file that we want to import. We'll start by writing the first line of the with statement in the following code cell. We'll use the open() function, setting the second parameter to “r”. Note: running this code will produce an error because it will only contain the first line of the with statement; we’ll complete this with statement in the task after this.
<p align="center">
<img src="https://i.imgur.com/Vfk2EzC.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

  <p align="center">
    Task 2:
  
  Now, we’ll use the .read() method to read the imported file, and we’ll store the result in a variable named text. Afterwards, we'll display the text and explore what it contains by running the cell.
  <p align="center">
<img src="https://i.imgur.com/a5LLGqE.png" height="80%" width="80%">

<p align="center">
    Task 3:
  
The output in the previous step is one big string. In this task, we’ll explore how you can split the string that contains the entire imported log file into a list of strings, one string per line. We'll use the .split() method to perform this split and then display the result.
  <p align="center">
<img src="https://i.imgur.com/oAocJfY.png" height="80%" width="80%">

<p align="center">
    Task 4:
  
There is a missing entry in the log file. We’ll need to account for that by appending it to the log file. We’re given the missing entry stored in a variable named missing_entry.
We'll use the .write() method and the parameter “a” in the open() function.
After the portion of the code that writes to the file, another with statement uses the .read() method to read the updated file into the text variable and then display it.
  <p align="center">
<img src="https://i.imgur.com/7VNLPSU.png" height="80%" width="80%">

<p align="center">
    Task 5:
  
 The next task we’re responsible for is creating a text file. This text file should include a list of IP addresses that are allowed to access restricted information. Documenting this in a text file will help us communicate our findings to our security team. We'll start by creating a variable named import_file that stores the name of the file, which should be “allow_list.txt”.
We’re also given a variable named ip_addresses that stores a string containing the IP addresses that are allowed.
  <p align="center">
<img src="https://i.imgur.com/cGoS1MV.png" height="80%" width="80%">

<p align="center">
    Task 6:  
  
 Our next goal is to create a with statement in order to write the IP addresses to the text file we created in the previous step.
We’ll first open the file using the “w” parameter. Then, we’ll write the IP addresses to the file.

Note that the code cell will contain a with statement that writes to a file but does not display information to the screen, so running it will not produce an output.
  <p align="center">
<img src="https://i.imgur.com/jH6kJDf.png" height="80%" width="80%">

<p align="center">
    Task 7:  
  
In this final step, we’ll complete the code we’ve been writing up to this point. We’ll add code to read the file containing IP addresses.

Let's complete a with statement that reads the text file and stores it in a new variable called text. Afterwards, we'll display the contents of text and run the cell.
  <p align="center">
<img src="https://i.imgur.com/MPhPvOV.png" height="80%" width="80%">

<p align="center">
    Conclusion:  
  
Python’s ability import and parse text files is a pivotal asset for cybersecurity analysts. This essential skill allows analysts to extract valuable insights from log files, network records, and system logs. By meticulously parsing these files, analysts can spot anomalies, uncover potential threats, and pinpoint vulnerabilities, which are critical steps in maintaining robust cybersecurity.

Python’s flexibility and extensive libraries make it an indispensable tool, providing analysts with the means to proactively defend against cyberattacks, investigate security incidents, and devise strategies to bolster overall digital protection.
     
<br /> 
<br />
    
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
