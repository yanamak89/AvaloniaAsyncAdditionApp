# AvaloniaAsyncAdditionApp

## Description

This application is implemented using **Avalonia UI** (a cross-platform alternative to WPF). The application demonstrates how to handle asynchronous operations triggered by a button click. It performs the addition of two numbers entered by the user in text fields and displays the result asynchronously.

---

## Features

- A user-friendly interface with two input fields, a button, and a result display area.
- Asynchronous handling of button click events using `Task.Run` and `ConfigureAwait(false)`.
- Real-time validation of user input and error handling.

---

## Requirements

- .NET 6.0 or higher
- Avalonia UI library
- A code editor like Visual Studio, Rider, or Visual Studio Code.

---

## Project Structure

- **UI Components**:
  - `Input1`: TextBox for the first number.
  - `Input2`: TextBox for the second number.
  - `AddButton`: Button to trigger the addition operation.
  - `ResultBox`: Read-only TextBox to display the result or error messages.
- **Addition Method**:
  - Performs synchronous addition of two numbers.
- **Async Event Handler**:
  - Calls the `Addition` method asynchronously using `Task.Run` and ensures efficient thread handling with `ConfigureAwait(false)`.

---

## How to Use
- Launch the application.
- Enter two numeric values in the provided input fields (Input1 and Input2).
- Click the "Add Numbers" button.
- The result of the addition will be displayed in the result box.
- If invalid input is provided, an error message will be shown in the result box.

---

## Expected Results
1. Valid Input
2. Input 5 in the first text box and 3 in the second text box.
3. Click the "Add Numbers" button.
4. The result 8 is displayed in the result box.

## Invalid Input
1. Input non-numeric values in any text box.
2. Click the "Add Numbers" button.
3. An error message appears: "Please enter valid numbers."

---

##  Key Concepts
1. **Asynchronous Programming**:

- The use of Task. Run to perform CPU-bound operations on a background thread.
- The await operator to wait for the operation to complete.
- Thread Management:
    ConfigureAwait(false) ensures that the continuation does not capture the current synchronization context, optimizing resource usage.

2. **Error Handling**:

- Input validation prevents non-numeric values from causing application crashes.
- Exceptions are caught and displayed gracefully in the result box.

3. **Conclusion**

This project demonstrates the effective use of Avalonia UI for building cross-platform desktop applications with asynchronous capabilities. It highlights the importance of Task.Run, ConfigureAwait, and robust error handling in modern application development.







