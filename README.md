# SIMPLE CALCULATOR USING PYTHON (CLI)
## 📘 OBJECTIVE
To create a command-line calculator supporting basic operations using Python,

---

## 🛠️ TOOLS USED
- **Language:** Python  
- **Platform:** IDLE / VS Code / Command Prompt  
- **Interaction Type:** CLI (Command Line Interface)

---

## 💻 PROGRAM CODE

```python
# Simple Calculator using functions, conditions, loop, and CLI interaction

def add(x, y):
    """Return the sum of x and y."""
    return x + y

def subtract(x, y):
    """Return the difference of x and y."""
    return x - y

def multiply(x, y):
    """Return the product of x and y."""
    return x * y

def divide(x, y):
    """Return the division of x by y. Handle division by zero."""
    if y == 0:
        return "Error: Cannot divide by zero!"
    return x / y

def calculator():
    print("Welcome to the Command-Line Calculator!")
    print("Operations:")
    print("1. Add (+)")
    print("2. Subtract (-)")
    print("3. Multiply (*)")
    print("4. Divide (/)")
    print("5. Exit")

    while True:
        choice = input("Select operation (1/2/3/4/5): ") 

        if choice == '5':
            print("Exiting calculator. Thank you!")
            break

        if choice not in ['1', '2', '3', '4']:
            print("Invalid choice! Please select from 1 to 5.")
            continue

        try:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))
        except ValueError:
            print("Invalid input! Please enter numeric values.")
            continue

        if choice == '1':
            print(f"{num1} + {num2} = {add(num1, num2)}")
        elif choice == '2':
            print(f"{num1} - {num2} = {subtract(num1, num2)}")
        elif choice == '3':
            print(f"{num1} * {num2} = {multiply(num1, num2)}")
        elif choice == '4':
            result = divide(num1, num2)
            print(f"{num1} / {num2} = {result}")

if __name__ == "__main__":
    calculator()
`````

----

## 📸 OUTPUT SCREENSHOT

<img width="660" height="533" alt="image" src="https://github.com/user-attachments/assets/f1942fb0-3de5-49c3-9364-c5c282dba88d" />

