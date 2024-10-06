# BPT Assignment Guide

This README provides step-by-step instructions on how to access, complete, and submit your BPT (Bi-weekly Points Test) assignments using the command line. Follow the steps below to set up your environment, view questions, create scripts, and submit your solutions.

---

## Table of Contents

- [Accessing BPT Questions](#accessing-bpt-questions)
- [Setting Up Your Assignment Directory](#setting-up-your-assignment-directory)
- [Viewing the Question](#viewing-the-question)
- [Creating and Editing `script.sh`](#creating-and-editing-scriptsh)
- [Making the Script Executable](#making-the-script-executable)
- [Running Your Script](#running-your-script)
- [Evaluating and Submitting Your Solution](#evaluating-and-submitting-your-solution)
- [Example Execution Output](#example-execution-output)
- [Notes](#notes)

---

## Accessing BPT Questions

1. **List Available Assignments:**

  Use the following command to list all available assignments in the `/opt/se2001/` directory:

   ```bash
   ls /opt/se2001/
   ```
   
2. **Copy Assignment Name:**

   - Find the assignment you need to work on
   - Copy its name for use in the next steps
---

## Setting Up Your Assignment Directory
1. **Navigate to Your SE2001 Directory:**
   
  Replace <roll.no> with your actual roll number
  ```
  cd /home/<roll.no>/se2001
  ```
2. **Create Assignment Directory:**

  You can name your assignment directory as ```assignment_<num>``` or ```BPT<num>_problem_<num>```
  ```
  mkdir assignment_<num>
  ```
  OR
  ```
  mkdir BPT<num>_problem_<num>
  ```
  Replace ```<num>``` with the appropriate assignment and problem number.

---

## Viewing the Question

1. **Navigate to Your Assignment Directory:**
  ```
  cd /home/<roll.no>/se2001/assignment_<num>
  ```
  OR
  ```
  cd /home/<roll.no>/se2001/BPT<num>_problem_<num>
  ```
2. **View the Question:**

  Use the ```synchro show command``` to display the assignment question:
  ```
  synchro show
  ```

---

## Creating and Editing script.sh

1. **Create or Open script.sh Using a Text Editor:**

  You can use any text editor you prefer. Here are two common options:
  - Using ```vim```:
  ```
  vim script.sh
  ```
    - To insert text, press i to enter Insert Mode.
    - Use arrow keys to navigate.
    - After editing, press Esc to exit Insert Mode.
    - Save and exit by typing ":wq" and pressing Enter.
  - Using nano:
  ```
  nano script.sh
  ```
    - Edit your script directly.
    - Save changes by pressing Ctrl + O, then Enter.
    - Exit the editor by pressing Ctrl + X.
    
2. **Write Your Script:**

  - Enter the required commands or code as per the assignment instructions.
  - Ensure your script is properly formatted and error-free.

3. **View the Script (Optional):**

To display the contents of your script:
```
cat script.sh
```

---

## Making the Script Executable

Change the permissions of ```script.sh``` to make it executable:
```
chmod +x script.sh
```

---

## Running Your Script

Execute your script using the following command:
```
./script.sh
```

---

## Evaluating and Submitting Your Solution

Use the ```synchro eval``` command to evaluate your script and submit your solution:
```
synchro eval
```

---

## Example Execution Output

An example of a successful execution and submission:
```
Passed tests: 28/28           
Public Test Cases: Evaluation successful.  
Public Test Cases: Submission successful.
Private Test Cases: No Private Testcases found.
Passed tests: Indicates the number of test cases your script passed.
```
Evaluation successful: Confirms that your code is correct.
Submission successful: Confirms that your submission was successful.
No Private Testcases found: Indicates there are no additional private test cases.


---

## Notes

- Important Commands:

  - ls: Lists directory contents.
  - cd: Changes the current directory.
  - mkdir: Creates a new directory.
  - synchro show: Displays the assignment question.
  - vim or nano: Opens a text editor to create or edit files.
  - chmod +x: Makes a script executable.
  - ./script.sh: Executes the script.
  - synchro eval: Evaluates and submits your solution.

- General Tips:

  - Always double-check your script for errors before making it executable.
  - Use comments in your script to document your code (optional but recommended).
  - Keep your workspace organized by using consistent naming conventions for directories and files.
  - If you encounter any errors during evaluation, revisit your script to troubleshoot and correct issues.
