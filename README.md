# This is a faulty calculator program for a Exercise given by Harry from Code with Harry Youtube Channel
# Coder - Praveen Singh Chauhan :)
# 45 * 3 = 555, 56+9=77, 56/6=4
# print(f'{num2} {num1}')

ope_cal = ""
num1, num2 = 0, 0

while ope_cal != "exit":
    ope_cal = input("What do you want > ").lower()
    if ope_cal == "exit":
        print("OK... we are ending this Calculator Program ......")
        break
    elif ope_cal == "+" or ope_cal == "-" or ope_cal == "*" or ope_cal == "/":
        num1 = int(input(" First Number >  "))
        num2 = int(input("Second Number >  "))
    else:
        print("you are doing mistake")
        print("its a '[Calculator]' so type operator i.e. + - * / ")
        print("*" * 50)

    if num1 == 45 and num2 == 3 and ope_cal == "*":
        print("Result is '[555]' ")
    elif num1 == 56 and num2 == 9 and ope_cal == "+":
        print("Result is '[77]' ")
    elif num1 == 56 and num2 == 6 and ope_cal == "/":
        print("Result is '[4]' ")
    elif ope_cal == "exit":
        break
    else:
        if ope_cal == "*":
            print(f'Result is "[{num1}*{num2}]"')
        elif ope_cal == "-":
            print(num1-num2)
        elif ope_cal == "+":
            print(num1 + num2)
        elif ope_cal == "*":
            print(num1 * num2)
        elif ope_cal == "/":
            print(num1 / num2)
# End of the program
