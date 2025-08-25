# Week 1 Homework Assignments: Introduction to MATLAB

## Global Requirements

- Add, commit, and push all deliverables to your `Week01` folder in your repository.

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

1. `report.txt` (1–2 paragraphs) describing the purpose of each interface component and your observations while exploring.

---

## 2. Basic Commands and Calculations

### Task

Practice using basic MATLAB commands and performing simple calculations.

### Requirements

- In the Command Window, perform basic arithmetic with variables.
- Use `clc` to clear the Command Window, `clear` to remove variables from the Workspace, and `whos` to inspect current variables.

### Deliverables

1. `week1_commands.m` with several arithmetic operations. Include comments explaining what each command does. Additionally, answer:
    - What does `clc` do?
    - What happens when you use `clear`?
    - What does `whos` display?

---

## 3. Using the Help System

### Task

Learn to use MATLAB’s help system to find information on specific commands and functions.

### Requirements

- Use the `help` command or MATLAB documentation to research: `fprintf`, `plot`, and `disp`.
- For each function:
  - Write a brief summary of what it does.
  - Provide an example of how to use it, with comments.
  - Experiment with a simple example (e.g., use `fprintf` to format and display a message; `plot` for a basic graph; `disp` to display text/variables).

#### Tips for Exploration

- Use `help disp` to learn about the `disp` function.
- `disp` is convenient for simple output without formatting.
- For formatted outputs (combining text and numbers), use `fprintf`.

### Deliverables

1. `functions_exploration.txt` with a summary and example for each function (`fprintf`, `plot`, `disp`).
2. `functions_exploration.m` demonstrating your examples.

---

## 4. Simple Script Creation

### Task

Write a simple script to perform a basic task; calculate the area of a rectangle.

### Requirements

- Create a new script `calculate_area.m`.
- Compute the area of a rectangle using variables for length and width.
- Print the result in a user-friendly format using `disp` or `fprintf` to match the example format:
  - The area of a <length> by <width> rectangle is <result>

### Tips
- Use `fprintf` for mixed text and numbers, or read `help disp` to see options for displaying values.
- To print numbers alongside text, format them (e.g., with `fprintf`).

### Example Output

```matlab
The area of a 5 by 10 rectangle is 50
```

### Deliverables

1. `calculate_area.m` with comments explaining each line. Test with different values for length and width and note the results in comments.

---

## 5. Bug Hunt Challenge

### Task

Practice debugging by identifying and fixing errors in a MATLAB script.

### Instructions

1. Copy the provided buggy MATLAB code to `buggy_script.m`.
2. Run it and observe any errors or unexpected behaviors.
3. Identify and fix the bugs (syntax, logic, or runtime). Use comments to explain each fix you make.

#### Example Buggy Script (buggy_script.m)

```matlab
% Task: Calculate the area of a circle and display the result

radius = 5
area = pi * radious^2
disp('The area of the circle is: ', area) % Incorrect use of disp function
```

### Deliverables

- `fixed_script.m` with comments explaining the errors you found and how you fixed them.
- `debugging_report.txt` including:
  - A summary of the errors encountered.
  - How you diagnosed and fixed them.
  - What you learned from the debugging process.

---

# Definition of Done
- You have a GitHub repository with `gberl001` invited as a collaborator.
- Your `Week01` folder contains at minimum:

  - `buggy_script.m`
  - `calculate_area.m`
  - `debugging_report.txt`
  - `fixed_script.m`
  - `functions_exploration.m`
  - `functions_exploration.txt`
  - `report.txt`
  - `week1_commands.m`
