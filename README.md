# Bank---Account---Management



🏦 Bank Account Management System Using Python

📌 Project Overview

The Bank Account Management System is a beginner-friendly Python project that demonstrates the core concepts of Object-Oriented Programming (OOP), including classes, objects, constructors, encapsulation, private attributes, and getter and setter methods.

The project allows users to create a bank account, view account details, check the current balance, and deposit money while validating the deposit amount.

🎯 Project Objectives

- Understand Python classes and objects.
- Implement constructors using "__init__()".
- Understand public and private attributes.
- Implement encapsulation to protect account balance data.
- Use getter and setter methods.
- Validate deposit amounts.
- Apply OOP concepts to a real-world banking example.

🛠️ Technologies Used

- Programming Language: Python
- Concepts: Object-Oriented Programming (OOP)
- Tools: VS Code / Jupyter Notebook / Google Colab
- Version Control: Git and GitHub

💻 Python Code

class bankaccount:

    def __init__(self, owner, balance):
        self.owner = owner
        self.__balance = balance

    def get_balance(self):
        return self.__balance

    def set_balance(self, amount):
        if amount > 0:
            self.__balance += amount
            print(
                f"Deposited ${amount}. "
                f"New balance: ${self.__balance}"
            )
        else:
            print("Invalid deposit amount")


# Create an account object
account = bankaccount("Durga", 1000)

# Display account details
print(f"Account owner: {account.owner}")
print(f"Initial Balance: ${account.get_balance()}")

# Deposit money
account.set_balance(1000)

📊 Sample Output

Account owner: Durga
Initial Balance: $1000
Deposited $1000. New balance: $2000

🔍 Project Explanation

1. Class and Object

The "bankaccount" class defines the structure of a bank account. The "account" object represents an individual account created from that class.

2. Constructor ("__init__")

The constructor initializes the account owner's name and the initial balance when an object is created.

3. Public Attribute

The "owner" attribute is public and can be accessed directly using "account.owner".

4. Private Attribute

The "__balance" attribute is private. Python uses name mangling to make direct access more difficult, encouraging access through methods.

5. Getter Method

The "get_balance()" method returns the current account balance without directly exposing the private attribute.

6. Deposit Method

The "set_balance()" method checks whether the deposit amount is positive. If it is, the amount is added to the existing balance.

Note: Although named "set_balance()", this method performs a deposit rather than setting an absolute balance. A more descriptive name would be "deposit()".

📈 Key Learning Outcomes

After completing this project, I learned how to:

- Create classes and objects in Python.
- Use constructors to initialize object attributes.
- Apply encapsulation using private attributes.
- Access private data through methods.
- Implement basic validation using conditional statements.
- Apply OOP concepts to a real-world banking scenario.

🚀 Future Improvements

The project can be enhanced by adding:

- A withdrawal feature.
- A balance validation system.
- Transaction history.
- Account number generation.
- A menu-driven interface.
- Exception handling.
- Unit tests for deposit and withdrawal operations.

👩‍💻 About Me

I am currently pursuing a Data Science course and developing my Python programming skills through practical projects.

This project is part of my journey to strengthen my understanding of Python and Object-Oriented Programming as I prepare for a career in Data Science.

Skills: Python | OOP | Encapsulation | Problem Solving

---

⭐ If you find this project useful, feel free to explore the code and share your feedback!