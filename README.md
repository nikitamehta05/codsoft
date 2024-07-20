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


