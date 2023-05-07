# Advanced-Calculator
A scientific calculator project in Python is a program that can perform various mathematical operations such as addition, subtraction, multiplication, division, exponentiation, logarithms, trigonometric functions, and more. This calculator is designed to be more advanced than a basic calculator, and it can perform more complex task.
import math

def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    if y == 0:
        return "Cannot divide by zero"
    else:
        return x / y

def power(x, y):
    return x ** y

def square_root(x):
    if x < 0:
        return "Invalid input"
    else:
        return math.sqrt(x)

print("Select operation:")
print("1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")
print("5. Power")
print("6. Square root")

choice = input("Enter your choice (1-6): ")

if choice in ('1', '2', '3', '4', '5'):
    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

if choice == '1':
    print(num1, "+", num2, "=", add(num1, num2))

elif choice == '2':
    print(num1, "-", num2, "=", subtract(num1, num2))

elif choice == '3':
    print(num1, "*", num2, "=", multiply(num1, num2))

elif choice == '4':
    print(num1, "/", num2, "=", divide(num1, num2))

elif choice == '5':
    print(num1, "**", num2, "=", power(num1, num2))

elif choice == '6':
    num = float(input("Enter number: "))
    print("Square root of", num, "=", square_root(num))

else:
    print("Invalid input")
