
# PLP Python Week 8 Final Project
# Personal Mini-Toolkit
# Name: Diclot Selemani

# PROJECT PLAN
# 1. Greeting Tool: Greets the user by name.
# 2. Even or Odd Checker: Checks whether a number is even or odd.
# 3. Shopping List Manager: Adds and displays shopping items.
# 4. Exit: Ends the program.
#
# Concepts used:
# Variables, input/output, if/elif/else, loops, lists, and comments.

# Store shopping items in a list
shopping_list = []

# Main menu loop
while True:
    print("\n===== PERSONAL MINI-TOOLKIT =====")
    print("1. Greeting Tool")
    print("2. Even or Odd Checker")
    print("3. Shopping List Manager")
    print("4. Exit")

    choice = input("Choose a tool (1-4): ").strip()

    # TOOL 1: Greeting Tool
    if choice == "1":
        name = input("Enter your name: ").strip()

        if name:
            print("Hello,", name + "! Welcome to your Personal Mini-Toolkit.")
        else:
            print("Please enter a name.")

    # TOOL 2: Even or Odd Checker
    elif choice == "2":
        try:
            number = int(input("Enter a whole number: "))

            if number % 2 == 0:
                print(number, "is an even number.")
            else:
                print(number, "is an odd number.")

        except ValueError:
            print("Invalid input. Please enter a whole number.")

    # TOOL 3: Shopping List Manager
    elif choice == "3":
        while True:
            print("\n--- SHOPPING LIST ---")
            print("1. Add item")
            print("2. Show items")
            print("3. Remove item")
            print("4. Return to main menu")

            action = input("Choose an action (1-4): ").strip()

            if action == "1":
                item = input("Enter item to add: ").strip()

                if item:
                    shopping_list.append(item)
                    print(item, "has been added.")
                else:
                    print("Item cannot be empty.")

            elif action == "2":
                if shopping_list:
                    print("\nYour shopping list:")
                    for item in shopping_list:
                        print("-", item)
                else:
                    print("Your shopping list is empty.")

            elif action == "3":
                item = input("Enter item to remove: ").strip()

                if item in shopping_list:
                    shopping_list.remove(item)
                    print(item, "has been removed.")
                else:
                    print("That item is not on your list.")

            elif action == "4":
                break

            else:
                print("Invalid choice. Please choose 1, 2, 3, or 4.")

    # TOOL 4: Exit
    elif choice == "4":
        print("Thank you for using the Personal Mini-Toolkit. Goodbye!")
        break

    else:
        print("Invalid choice. Please select a number from 1 to 4.")
