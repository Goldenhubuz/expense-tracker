# Expense Tracker CLI

Expense Tracker CLI is a simple command-line interface (CLI) application for managing personal expenses. This tool allows you to add, delete, and view expenses right from your terminal, making it easy to keep track of your spending.

## 🔗 Project Links

- **Project Page**: [Expense Tracker project page](https://roadmap.sh/projects/expense-tracker)
- **Submission Solution**: [My Expense Tracker solution submission](https://roadmap.sh/projects/expense-tracker/solutions?u=6740b9f45434bf319a47ee77)

## 🚀 Features

- ✅ **Add Expenses**: Quickly add new expenses with a description and amount.
- ❌ **Delete Expenses**: Remove expenses by their ID.
- 📋 **List Expenses**: Display all recorded expenses in a formatted table.
- 📊 **Monthly Summary**: View a summary of total expenses for a specific month or all months.

---

## 📥 Installation

1️⃣ **Clone the Repository**:
```bash
git clone https://github.com/goldendevuz/expense-tracker.git
```

2️⃣ **Navigate to the Project Directory**:
```bash
cd expense-tracker
```

3️⃣ **Install Dependencies**:
Ensure you have Python installed. Then, install the required Python packages:
```bash
make i
```

4️⃣ **Create an Alias for CLI**:

To use the `expense-tracker` command, run:
```bash
alias expense-tracker="python main.py"
```

This will allow you to execute CLI commands using `expense-tracker` within the current terminal session.

---

## 📌 Available Commands

### 1️⃣ Add a New Expense

Use the `add` command to create a new expense:

```bash
expense-tracker add --description "Lunch" --amount 20
expense-tracker add --description "Dinner" --amount 10
```

💡 **Result**:
```bash
Expense added successfully (ID: 1)
Expense added successfully (ID: 2)
```

---

### 2️⃣ List Expenses

To display all recorded expenses:
```bash
expense-tracker list
```

📋 **Output**:
```
+----+------------+-------------+--------+
| ID |    Date    | Description | Amount |
+----+------------+-------------+--------+
| 1  | 2025-02-16 |    Lunch    |   20   |
| 2  | 2025-02-16 |    Dinner   |   10   |
+----+------------+-------------+--------+
```

---

### 3️⃣ Delete an Expense

To delete an expense by its ID:
```bash
expense-tracker delete --id 2
```

🗑️ **Result**:
```bash
Expense deleted successfully
```

---

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## ✉️ Contact

📧 For questions and feedback, contact: [goldendevuz@gmail.com](mailto:goldendevuz@gmail.com)

---

🚀 **Happy expense tracking!**
