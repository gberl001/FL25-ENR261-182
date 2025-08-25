# Week 8 Homework Assignments: MATLAB App Designer and Symbolic Math

## Global Requirements

* All deliverables shall be added, committed, and pushed to your Week9 folder in your repository.
* Include your name and the names of anyone who assisted you in the following format:

```matlab
% Student: Firstname Lastname
% Assisted by: Firstname Lastname, etc.
```

* Provide comments explaining each part of your code.
* Ensure proper functionality and usability of your MATLAB apps.
* Ensure inputs and outputs are handled properly and tested with different scenarios.
* For symbolic operations, use MATLAB’s symbolic toolbox functions (e.g., sym, diff, int, etc.).

## 1. Function Plotter with Symbolic Expressions

### Task

Create an app using MATLAB App Designer that takes a user-input symbolic expression and plots the function over a given
range.

**App Components**:

1. Input Field for Symbolic Expression:
    * The user should be able to input a symbolic expression (e.g., `x^2 + 3*x + 2`).
2. Input Fields for Plot Range:
    * Two input fields to specify the start and end of the range for the x-axis.
3. Plot Button:
    * A button that, when pressed, generates and displays the plot of the symbolic expression over the specified range.
4. Axes Element:
    * An axes component where the plot of the symbolic function will be displayed.

**Instructions**:

1. Create the App:
    * Use MATLAB App Designer to design the user interface.
    * Use the sym function to convert user input into a symbolic expression.
    * Use `fplot` to plot the symbolic expression over the user-defined range.
2. Error Handling:
    * Ensure your app handles invalid symbolic expressions and displays an error message using a dialog box.
3. Testing:
    * Test the app with various expressions, including polynomials, trigonometric, and exponential functions.

### Example Output

When running your app, the user should be able to input a function like x^3 + 2*x - 5, define the range as -10 to 10,
and see the corresponding plot displayed on the axes.

### Deliverables

	1.	Submit the .mlapp file for your app (e.g., FunctionPlotter.mlapp).
	2.	Include comments explaining each part of your code and UI components.

## 2: Symbolic Differentiation and Integration App

### Task

Create an app using MATLAB App Designer that allows users to input a symbolic expression and choose whether to
differentiate or integrate the expression symbolically.

**App Components**:

1. Input Field for Symbolic Expression:
    * The user should be able to input a symbolic expression (e.g., x^2 + 3*x).
2. Radio Buttons for Operation:
    * The user selects either “Differentiate” or “Integrate.”
3. Variable Dropdown:
    * A dropdown menu to select the variable with respect to which the differentiation or integration will be
      performed (e.g., x, y).
4. Result Display:
    * Display the resulting symbolic expression after the chosen operation.
5. Plot Button:
    * A button to plot both the original and the derived/integrated function over a given range.

**Instructions**:

1. Create the App:
    * Use MATLAB App Designer to design the user interface.
    * Use diff for symbolic differentiation and int for symbolic integration.
    * Allow users to select the variable from a dropdown and apply the operation accordingly.
2. Plot the Functions:
    * Plot both the original function and the derived or integrated function on the same axes over a user-defined range.
3. Error Handling:
    * Display an error message if the user input is not a valid symbolic expression.
4. Testing:
    * Test the app with various symbolic expressions and variables, and ensure both differentiation and integration
      operations work correctly.

### Example Output

The app should allow a user to input `x^2 + 2*x + 1`, choose “Differentiate”, and display the result `2*x + 2`. The plot
should show both the original function and its derivative.

Deliverables

1. Submit the `.mlapp` file for your app (e.g., `SymbolicDiffIntApp.mlapp`).
2. Include comments explaining each part of your code and UI components.

## 3. Unit Converter App

### Task

Create an app using MATLAB App Designer that converts between common units of measurement across several categories

**App Components**:

1. Category Selection (Drop-Down):
    * A drop-down menu allowing users to choose a unit category (e.g., Length, Temperature, Weight). See the categories and conversions below.
2. Unit Selection (Two Drop-Downs):
    * Two drop-downs to select the source unit and the target unit, populated based on the chosen category.
      * Example: If the user chooses length, only length related units should appear in the dropdown. See the categories and conversions below.
3. Input Field:
    * A numeric input where the user enters the value to convert.
4. Convert Button:
    * A button to trigger the conversion logic and display the result.
5. Result Display:
    * A label or text area to display the converted result.

**Instructions**:

1. Create the App:
    * Use MATLAB App Designer to design the user interface with appropriate layout and labeling.
    * Populate unit options dynamically based on the selected category.
    * Use basic formulas for conversions (e.g., °C to °F, meters to feet, grams to pounds). See the categories and conversions below.
2. Handle Conversions:
    * Implement the conversion logic in a callback function triggered by the button. See the categories and conversions below.
    * Display the result in the result label or text area.
3. Error Handling:
    * Display an error message for invalid input values or if a conversion is unsupported.
4. Testing:
    * Test the app with multiple values and categories (e.g., convert 100°C to °F, 5 meters to feet, 1000 grams to pounds).

**Category: Length**

| Unit        | Abbreviation | To Meters (×)     | From Meters (÷)    |
|-------------|--------------|-------------------|--------------------|
| meter       | m            | 1                 | 1                  |
| kilometer   | km           | 1000              | 1000               |
| inch        | in           | 0.0254            | 0.0254             |
| foot        | ft           | 0.3048            | 0.3048             |
| mile        | mi           | 1609.344          | 1609.344           |
**Category: Temperature**

| From \ To   | Celsius                | Fahrenheit                   | Kelvin                    |
|-------------|------------------------|-------------------------------|---------------------------|
| Celsius     | x                      | (x × 9/5) + 32                | x + 273.15                |
| Fahrenheit  | (x - 32) × 5/9         | x                             | ((x - 32) × 5/9) + 273.15 |
| Kelvin      | x - 273.15             | ((x - 273.15) × 9/5) + 32     | x                         |
**Category: Weight**

| Unit        | Abbreviation | To Grams (×)      | From Grams (÷)      |
|-------------|--------------|-------------------|---------------------|
| gram        | g            | 1                 | 1                   |
| kilogram    | kg           | 1000              | 1000                |
| pound       | lb           | 453.59237         | 453.59237           |
| ounce       | oz           | 28.3495           | 28.3495             |

### Example Output

The user should be able to select “Temperature”, choose “Celsius” as the source and “Fahrenheit” as the target, enter `100` as the value, and get the result `212 °F`.

### Deliverables

1. Submit the `.mlapp` file for your app (e.g., `UnitConverter.mlapp`).
2. Include comments explaining each part of your code and UI components.

## Definition of Done

Your `Week09` folder shall contain at minimum the following files:

* Week09/
  * `FunctionPlotter.mlapp`
  * `SymbolicDiffIntApp.mlapp`
  * `UnitConverter.mlapp`

Ensure that each app is well-documented, functions correctly, and follows good coding practices.

# Additional Instructions

* **Testing**:
    * While explicit test scripts are not provided, test each app by inputting various symbolic expressions.
    * Ensure that invalid inputs are handled gracefully with error messages.
* **Plotting**:
    * For assignments involving plots, ensure the plots are properly labeled with titles, axis labels, and legends where
      appropriate.
    * Use grid lines and appropriate line styles for clarity where needed.
* **Have Fun**:
    * There is no requirement on the appearance of your applications
    * Apply any layout, coloring, or basic user experience (UX) that you feel benefits the user.

## Tips

- **Handling Errors with Symbolic Expressions**: Use `try-catch` to handle unknown input errors for symbolic
  expressions. For example:

    ```matlab
    try
        expr = sym(input);
        % Your code to process and plot the expression
    catch
        errordlg('There was an error with your input, please try again.');
    end
    ```

- **Use Error Dialogs**: Instead of printing errors to the console, use `errordlg` to show error messages to the user in
  a dialog box. This enhances the user experience in App Designer.

- **Debugging**: Use `disp` or `fprintf` statements to help debug and trace variable values or flow of execution. For
  example, you can print key variables before plotting:

    ```matlab
    fprintf('Plotting function: %s\n', char(expr));
    ```

- **Using `matlabFunction`**: When working with symbolic expressions, you can’t plot them directly using standard
  plotting functions. First, convert symbolic expressions into function handles using `matlabFunction`. For example:

    ```matlab
    f_handle = matlabFunction(expr);
    ```

  This allows you to pass the symbolic expression to plotting functions like `fplot` or use it in other numerical
  computations. For instance:

    ```matlab
    fplot(f_handle, [x_start, x_end]);
    ```

- **Using `fplot` for Symbolic Functions**:  
  The `fplot` function simplifies plotting symbolic expressions. It automatically handles the evaluation and range of
  the plot. If you’ve used `matlabFunction` to convert your symbolic expression into a function handle, you can pass it
  directly to `fplot`. For example:

    ```matlab
    fplot(@(x) sin(x), [-pi, pi]);  % for predefined functions
    fplot(f_handle, [-10, 10]);     % for symbolic expressions
    ```

  The advantage of `fplot` is that it automatically adjusts the plot resolution and avoids the need to manually evaluate
  the function at discrete points.