def calculator():
  print("This is a simple calculator")
  try:
    num1 = float(input("Enter Number 1:"))
    num2 = float(input("Enter Number 2:"))
    operation = input("Choose an operation (+, -, *, /):")
    if operation == '+':
      result = num1 + num2
    elif operation == '-':
      result = num1 - num2
    elif operation == '*':
      result = num1 * num2
    elif operation == '/':
      if num2 == 0:
        result = "Dvision error!"
      else:
        result = num1 / num2
    else:
      result = "Invalid Opertion"
    print(f"The result is: {result} ")
  except ValueError:
    print("Invalid input. Please enter a valid number")
calculator()
