# calculator
Simple caculator
# PLP ASSIGNMENT ON PYTHON
# simple calculator programe 
# Get user input
num1 = float(input("Enter the first number: "))
num2 = float(input("Enter the second number: "))
operation = input("Enter an operation (+, -, *, /): ")

#Perform the calculation based on the operation\
if operation == '+':
    result = num1 + num2
    print(f"The result of {num1} + {num2} is {result}")
elif operation == '-':
    result = num1 - num2
    print(f"The result of {num1} - {num2} is {result}")
elif operation == '*':
    result = num1 * num2
    print(f"The result of {num1} * {num2} is {result}")
elif operation == '/': 
    #check for division by zero
    if num2 !=0:
        result = num1 / num2
        print(f"The result of {num1} / {num2} is {result}")
    else:
        print ("Error: Division by Zero is not allowed.")
else:
    print("Error: Invalid operation, please enter +, -, *, or /.")
