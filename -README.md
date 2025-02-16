# Expense Tracker CLI

Expense Tracker CLI is a simple command-line interface (CLI) application for managing personal expenses. This tool allows you to add, delete, and view expenses right from your terminal, making it easy to keep track of your spending.

## Project Links

- **Project Page**: Visit the [Expense Tracker project page](https://roadmap.sh/projects/expense-tracker) for more information.
- **Submission Solution**: View my [Expense Tracker solution submission](https://roadmap.sh/projects/expense-tracker/solutions?u=6740b9f45434bf319a47ee77).

## Features

- **Add Expenses:** Quickly add new expenses with a description and amount.
- **Delete Expenses:** Remove expenses by their ID.
- **List Expenses:** Display all recorded expenses in a formatted table.
- **Monthly Summary:** View a summary of total expenses for a specific month or all months.

## Installation

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/goldendevuz/expense-tracker.git
   ```
   
2. **Navigate to the Project Directory:**
   ```bash
   cd ExpenseTracker
   ```

3. **Install Dependencies:**
   Ensure you have Python installed. Then, install the required Python packages:
   ```bash
   make i
   ```

4. **Link the CLI to the custom commnad**:

   To link as `expense-tracker` command, run:

   ```bash
   alias expense-tracker="python main.py"
   ```

   This will make the `expense-tracker` command available in this folder.


### Available Commands

#### 1. Add a New Expense

Use the `add` command to create a new expense.

```bash
expense-tracker add --description <description> --amount <amount>
expense-tracker add --description "Lunch" --amount 20
expense-tracker add --description "Dinner" --amount 10
```

**Result**:

```bash
Expense added successfully (ID: 1)
Expense added successfully (ID: 2)
```

#### 2. Listing Expenses

List all recorded expenses:
```bash
expense-tracker list

+----+------------+-------------+--------+
| ID |    Date    | Description | Amount |
+----+------------+-------------+--------+
| 1  | 2025-02-16 |    Lunch    |   20   |
| 2  | 2025-02-16 |    Dinner   |   10   |
+----+------------+-------------+--------+
```

#### 3. Delete a Expense

Use the `delete` command to remove a expense by its ID.

```bash
expense-tracker delete --id <expense_id>
expense-tracker delete --id 2
```

**Result**:

```bash
Expense deleted successfully
```

#### 4. Mark a Expense as In Progress

Use the `mark-in-progress` command to update the status of a expense to `in-progress`.

```bash
expense-cli mark-in-progress <expense_id>
```

**Result**:

```bash
expense-cli mark-in-progress 1
```

#### 5. Mark a Expense as Done

Use the `mark-done` command to update the status of a expense to `done`.

```bash
expense-cli mark-done <expense_id>
```

**Result**:

```bash
expense-cli mark-done 1
```

#### 6. List All Expenses

Use the `list` command to view all expenses.

```bash
expense-cli list
```

**Result**:

```bash
expense-cli list
```

## Usage

To start using the Expense Tracker CLI, simply run the Python script with the desired commands.

### Adding an Expense

Add a new expense by providing a description and an amount:
```bash
expense-tracker add --description "Lunch" --amount 20
# Expense added successfully (ID: 1)

expense-tracker add --description "Dinner" --amount 10
# Expense added successfully (ID: 2)
```

### Deleting an Expense

Delete an expense by specifying its ID:
```bash
python main.py delete <expense_id>
```

### Viewing a Monthly Summary

View a summary of expenses for a specific month:
```bash
python main.py summary 5  # For May
```

View a summary of expenses for all months:
```bash
expense-tracker summary
# Total expenses: $30
```

## Expense File

All expenses are stored in an `expenses.json` file in the project directory. The structure of this file is managed automatically by the CLI.

### Expense Structure

Each expense has the following attributes:
- `id`: Unique identifier for the expense.
- `date`: The timestamp when the expense was added.
- `description`: A brief description of the expense.
- `amount`: The amount spent on the expense.

## Diagram

![Expense Tracker Diagram](./ExpenseTracker.svg)

## Idea Source

The idea for the Expense Tracker CLI project was inspired by [roadmap.sh's Expense Tracker project](https://roadmap.sh/projects/expense-tracker). Visit the link to see more details and learn about similar project ideas.

## Contributing

Contributions are welcome! If you find any issues or have suggestions for improvements, feel free to open an issue or submit a pull request.

1. Fork the repository.
2. Create a new branch for your feature or fix.
3. Commit your changes.
4. Push to the branch.
5. Open a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contact

For any questions or feedback, please contact [goldendevuz@gmail.com](mailto:goldendevuz@gmail.com).

---

Happy expense tracking!