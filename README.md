# Arthmetic.py
I have given arthmetic opertor in python with user input.
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y != 0:
        return x / y
    else:
        return "Error! Division by zero."

# Display menu
print("Select an operation:")
print("1. Add")
print("2. Subtract")
print("3. Multiply")
print("4. Divide")

# Take user input for the choice of operator
choice = input("Enter choice (1/2/3/4): ")

# Take user input for operands
num1 = float(input("Enter the first operand: "))
num2 = float(input("Enter the second operand: "))

# Perform the chosen operation
if choice == '1':
    print(f"The result is: {add(num1, num2)}")
elif choice == '2':
    print(f"The result is: {subtract(num1, num2)}")
elif choice == '3':
    print(f"The result is: {multiply(num1, num2)}")
elif choice == '4':
    print(f"The result is: {divide(num1, num2)}")
else:
    print("Invalid input! Please choose a valid operation.")
