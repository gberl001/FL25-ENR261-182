# Week 1 Homework Assignments: Introduction to MATLAB

## Global Requirements

* All deliverables shall be `added`, `committed`, and `pushed` to your `Week1` folder in your repository.

## 1. Exploring the MATLAB Interface

### Task

Perform a guided tour of the MATLAB interface.

### Instructions

- Open MATLAB and explore the different components:
    - **Command Window**: Use it to enter commands and see immediate results.
    - **Workspace**: Check how variables appear as you create them.
    - **Editor**: Create a new script file and save it with a name like `week1_script.m`.
    - **Command History**: Observe how it records the commands you enter.

### Deliverables

1. Write a brief report `report.txt` (1-2 paragraphs) describing the purpose of each part of the interface and any
   observations you made while exploring.

---

## 2. Basic Commands and Calculations

### Task

Practice using basic MATLAB commands and performing simple calculations.

### Requirements

- In the Command Window, try performing basic arithmetic using different variables.
- Use commands like `clc` to clear the Command Window, `clear` to remove variables from the Workspace, and `whos` to
  see the current variables.

### Deliverables

1. Submit a script file (`week1_commands.m`) that includes several arithmetic operations. Include comments explaining
   what each command does. Additionally, answer the following questions:
    - What does `clc` do?
    - What happens when you use `clear`?
    - What does `whos` display?

---

## 3. Using the Help System

### Task

Learn to use MATLAB’s help system to find information on specific commands and functions.

### Requirements
* Use the `help` command or MATLAB documentation to research the following three MATLAB functions: `fprintf`, `plot`,
  and `disp`.
* For each function:
    * Write a brief summary of what it does.
    * Provide an example of how to use it, including comments explaining your understanding.
    * Experiment with the function in MATLAB by creating a simple example (e.g., use `fprintf` to format and display a
      message, use `plot` to create a basic graph, use `disp` to display text, variables, or a combo).

#### Tips for Exploration

* Use the command `help disp` in the Command Window to learn about the `disp` function.
* Think about how you might want to display information or variables to the user. `disp` is often used for simple output
  without formatting.
* For more complex outputs, you might explore how `fprintf` differs from `disp`.

### Deliverables

1. Submit a report (`functions_exploration.txt`) with a summary and example for each
   function (`fprintf`, `plot`, `disp`).
1. Include a simple MATLAB script (`functions_exploration.m`) that demonstrates your examples.

---

## 4. Simple Script Creation

### Task

Write a simple script to perform a basic task; calculate the area of a rectangle.

### Requirements

- Create a new script in the MATLAB Editor and save it as `calculate_area.m`.
- The script should calculate the area of a rectangle using variables for length and width.
- Print the result in a user-friendly format using `disp` or, `fprintf` to achieve the output shown in the example. 
  - The area of a \<length\> by \<width\> rectangle is \<result\>

### Tips
  - You will need to read the `help` on `disp` to learn how to display text and numbers together.
  - In order to print numbers and text (strings), you need to convert numbers to a string

### Example Output

```matlab
The area of a 5 by 10 rectangle is 50
```

### Deliverables

1. Submit the script file (`calculate_area.m`). Include comments explaining each line of your code. Test the script with
   different values for length and width, and note the results.

---

## 5. Bug Hunt Challenge

### Task

Practice debugging by identifying and fixing errors in a MATLAB script.

### Instructions

1. Copy the provided buggy MATLAB code to a script file named `buggy_script.m`.
1. Open the script in the MATLAB Editor and try running it. Observe the errors or unexpected behaviors.
1. Identify the bugs in the script and fix them. The bugs could be syntax errors, logical errors, or runtime errors. Use
   comments to explain each fix you make.

#### Example Buggy Script (buggy_script.m)

```matlab
% Task: Calculate the area of a circle and display the result

radius = 5
area = pi * radious^2
disp('The area of the circle is: ', area) % Incorrect use of disp function
```

### Deliverables

* Submit the corrected script file (`fixed_script.m`). Include comments explaining the errors you found and how you fixed them.
* Write a short report (`debugging_report.txt`) containing the following
  * Summarize the errors you encountered.
  * Explain how you found the solution to fix them.
  * Explain what you learned from the debugging process.

---

# Definition of Done
1. You shall have a Github Repository set up with `gberl001` invited as a collaborator.
2. Your Week1 Folder shall have the following files
   * buggy_script.m
   * calculate_area.m
   * debugging_report.txt
   * fixed_script.m
   * functions_exploration.m
   * functions_exploration.txt
   * Report.txt
   * week1_commands.m