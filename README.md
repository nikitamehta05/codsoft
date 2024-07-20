#CODESOFT
TASK 1:
#python program to make a simple calculator for two numbers

    def CALCULATOR():
     n1=int(input("Enter first number"))
     n2=int(input("Enter second number"))
     if choice=='1':
       print("Addition:",n1+n2)
     elif choice=='2':
       print("Subtraction:",n1-n2)
     elif choice=='3':
       print("Multiplication:",n1*n2)
     elif choice=='4':
       if n2!=0:
         print("Division:",n1/n2)
       else:
         print("Division by zero is not allowed.")
     else:
        print("ENTER VAILD CHOICE")
   
    print("SIMPLE CALCULATOR")
    print("1.Add(+)")
    print("2.Sub(-)")
    print("3.Mul(*)")
    print("4.div(/)")
    choice=input("Enter your choice(1,2,3,4):")
    CALCULATOR()
TASK 2:
#Python code for a password generator application:

    import random
    import string

    def password_generator():
      length = int(input("Enter the desired length of the password (8-200): "))
      if length < 8 or length > 200:
       print("Password length must be between 8 and 20 characters.")
       return

      complexity = input("Choose password complexity (weak/medium/strong): ")

      characters = string.ascii_lowercase
       if complexity in ['medium', 'strong']:
         characters += string.ascii_uppercase
       if complexity in ['strong']:
        characters += string.digits + string.punctuation

      password = ''.join(random.choice(characters) for _ in range(length))
      print("Generated Password: ", password)
     password_generator()

TASK 3:
#Python code for a Rock-Paper-Scissors game:

     import random

    def play_game():
     while True:
      user_choice = input("Enter your choice (rock/paper/scissors) or 'q' to quit: ").lower()
      if user_choice == 'q':
       break

     if user_choice not in ['rock', 'paper', 'scissors']:
      print("Invalid choice. Please enter rock, paper, or scissors.")
      continue

     computer_choice = random.choice(['rock', 'paper', 'scissors'])
     print(f"\nComputer chose: {computer_choice}\n")

     if user_choice == computer_choice:
      print(f"Both players selected {user_choice}. It's a tie!")
     elif user_choice == 'rock':
      if computer_choice == 'scissors':
        print("Rock smashes scissors! You win!")
      else:
        print("Paper covers rock! You lose.")
     elif user_choice == 'paper':
      if computer_choice == 'rock':
        print("Paper covers rock! You win!")
      else:
        print("Scissors cuts paper! You lose.")
     elif user_choice == 'scissors':
      if computer_choice == 'paper':
        print("Scissors cuts paper! You win!")
      else:
        print("Rock smashes scissors! You lose.")

     play_again = input("\nPlay again? (yes/no): ")
     if play_again.lower() != 'yes':
      break

    play_game()






