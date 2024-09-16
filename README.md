# Employee-register
Employee register -(Angular)

# Employee Register

**Employee Register** is an Angular application designed to manage a list of employees. This project allows users to view, add, edit, and delete employee records, each of which includes personal details and a photo.

## Features

- **Employee List**: Display all employees in a scrollable grid. Employees are sorted by their date of joining, with options to sort by name, date of joining (DoJ), or date of birth (DoB).
- **Add Employee**: Form to add new employee details with validations.
- **Edit Employee**: Form to edit existing employee details.
- **Delete Employee**: Confirm deletion of an employee via a pop-up dialog.

## Screens

### Screen 1: Employee List

- Displays a list of employees in a grid format.
- Each employee card includes a photo, full name, and date of joining.
- Employees are initially sorted by the date of joining, with options to sort by name, DoJ, or DoB.
- Tapping on an employee card takes the user to the edit screen.
- A blue circle with a white plus sign at the bottom right allows users to add a new employee.

### Screen 2: Add an Employee

- **Form Fields**:
  - Full Name (capitalized)
  - Nickname (one word)
  - Date of Joining (21st century, not future)
  - Date of Birth (within the last 100 years)
  - Designation
  - Current Salary (positive floating point number)
  - Photo (JPEG, max 2MB, unique)
  - Personal Email Address (validated)
  - Mobile Number (validated using libphonenumber)
  - Year of Graduation (four-digit integer, not more than 80 years old)
- Validation is implemented for all fields with meaningful error messages.
- Two buttons at the bottom right: "Discard" and "Add".

### Screen 3: Edit Employee

- Similar to the add employee form.
- Includes "Revert", "Save", and "Delete" buttons at the bottom right.
- Edits are saved or reverted, and the user returns to the employee list with updated information.

### Screen 4: Delete Employee

- Pop-up dialog to confirm deletion of an employee.
- Shows all details of the employee and includes "Cancel" and "Delete" buttons.

## Setup and Installation

1. **Clone the repository**:
    ```bash
    git clone https://github.com/your-username/employee-register.git
    cd employee-register
    ```

2. **Install dependencies**:
    ```bash
    npm install
    ```

3. **Run the application**:
    ```bash
    ng serve
    ```

4. **Navigate to** `http://localhost:4200` in your browser to view the application.

## Configuration

Ensure you have Angular CLI installed. You can install it globally using:
```bash
npm install -g @angular/cli
