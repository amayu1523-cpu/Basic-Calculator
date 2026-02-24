# Basic-Calculator

def calculator():
    while True:
        print("=" * 40)
        print("         BASIC CALCULATOR")
        print("=" * 40)
        print("1. Addition")
        print("2. Subtraction")
        print("3. Multiplication")
        print("4. Division")
        print("5. Exit")
        print("=" * 40)

        choice = input("Enter your choice: ")

        if choice == "5":
            print("Thank You!")
            break

        if choice in ["1", "2", "3", "4"]:
            num1 = float(input("Enter first number: "))
            num2 = float(input("Enter second number: "))

            if choice == "1":
                result = num1 + num2
                print("Result =", result)

            elif choice == "2":
                result = num1 - num2
                print("Result =", result)

            elif choice == "3":
                result = num1 * num2
                print("Result =", result)

            elif choice == "4":
                if num2 != 0:
                    result = num1 / num2
                    print("Result =", result)
                else:
                    print("Cannot divide by zero!")

        else:
            print("Invalid Choice!")

        input("\nPress Enter to continue...")

calculator()
