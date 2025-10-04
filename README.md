
# Task 8 – Stored Procedures and Functions

##  Introduction

In SQL, **Stored Procedures** and **Functions** are reusable database objects that help modularize logic and improve efficiency.

* **Stored Procedure**: A block of SQL code that can perform multiple operations such as insert, update, delete, or select. Procedures can take **IN/OUT parameters** but **cannot return values directly**.
* **Function**: A block of SQL code that always **returns a single value** (scalar or table). Functions are often used for calculations, validations, and returning computed results.

##  Difference Between Procedure and Function

| Feature      | Stored Procedure                             | Function                       |
| ------------ | -------------------------------------------- | ------------------------------ |
| Return Value | Cannot return directly (only via OUT params) | Must return a value            |
| Usage        | Insert, Update, Delete, Business logic       | Calculations, return data      |
| Called From  | Executed using `CALL`                        | Used inside queries (`SELECT`) |
| Parameters   | IN, OUT, INOUT                               | Only IN                        |
| Transactions | Can commit/rollback                          | Cannot commit/rollback         |

---

## 🛠 Key Concepts

1. **IN Parameter** → Passes a value into a procedure/function.
2. **OUT Parameter** → Returns a value from a procedure.
3. **RETURN** → Mandatory in functions, optional in procedures.
4. **Deterministic Functions** → Return the same result for the same input.

---

## Examples Used

In this task, we worked on an **Employee Table** with the following fields:

* **Emp_id** → Employee ID
* **Emp_name** → Employee Name
* **Emp_age** → Employee Age
* **Emp_salary** → Employee Salary

I have created:

* **4 Stored Functions** → To calculate age, salary, name, and seniority check.
* **4 Stored Procedures** → To insert, update, delete, and display employees.


## Benefits of Stored Routines

* **Reusability**: Code can be reused multiple times.
* **Modularity**: Breaks large SQL operations into small blocks.
* **Maintainability**: Easy to update logic in one place.
* **Performance**: Precompiled and faster execution.
* **Security**: Access can be restricted via permissions.



