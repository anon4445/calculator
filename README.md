# Simple Calculator Program in Python

This Python script implements a basic calculator that allows users to perform arithmetic operations on two input numbers.

## How to Use

1. Run the Python script.
2. Enter the first number when prompted.
3. Enter the second number when prompted.
4. Choose an arithmetic operation:
   - Type `1` for addition.
   - Type `2` for subtraction.
   - Type `3` for multiplication.
   - Type `4` for division.

The program will execute the chosen arithmetic operation on the entered numbers and display the result.

## Code Explanation

The script performs the following steps:

1. **User Input**:
   - Prompt the user to enter two numbers.
   - Convert the inputs to floating-point numbers.

2. **Display Options**:
   - Display a menu of arithmetic operations.

3. **User Choice**:
   - Prompt the user to choose an arithmetic operation.

4. **Perform Calculation**:
   - Based on the user's choice, perform the corresponding arithmetic operation:
     - Addition, subtraction, multiplication, or division.
     - Handle division by zero.

5. **Output Result**:
   - Display the result of the chosen arithmetic operation.

## Sample Usage

```python
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print("\n1. Addition")
print("2. Subtraction")
print("3. Multiplication")
print("4. Division")

choice = input("\nEnter your choice (1/2/3/4): ")

if choice == '1':
    print("The result is:", num1 + num2)
elif choice == '2':
    print("The result is:", num1 - num2)
elif choice == '3':
    print("The result is:", num1 * num2)
elif choice == '4':
    if num2 != 0:
        print("The result is:", num1 / num2)
    else:
        print("Error! Division by zero is not allowed.")
else:
    print("Invalid input")
