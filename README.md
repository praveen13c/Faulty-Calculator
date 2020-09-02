# Exercise to make a Faulty Calculator, Deliberately  give wrong result for
# 45 * 3 = 555, 56+9=77, 56/6=4 faulty calculate have to calculate this else right calculation
# Problem given by Harry from Code with Harry Youtube Channel (HarisAK)
# Coder - Praveen Singh Chauhan (Technology Video Network - Youtube Channel ,
# GAMP Aaryawarti Films - Film Production & Youtube Channel)
# Link of Youtube - https://www.youtube.com/TechnologyVideoNetwork , https://www.youtube.com/gampaaryawartifilms
# Facebook - https://www.facebook.com/praveen13c
# Twitter - https://twitter.com/praveen13c , https://twitter.com/tvnutube
# Linkedin -  https://www.linkedin.com/in/impraveenchauhan

ope_cal = ""
num1, num2 = 0, 0

while ope_cal != "exit":
    print("=" * 50)
    print("type 'exit' to end program or math operator like + - * / **")
    ope_cal = input("What do you want to do > ").lower()

    if ope_cal == "exit":
        print("OK... we are ending this Calculator Program ......")
        break
    elif ope_cal == "+" or ope_cal == "-" or ope_cal == "*" or ope_cal == "/" or ope_cal == "%" or ope_cal == "**":
        num1 = input(" First Number >  ")

        try:
            num1 == int(num1)
        except Exception as err_num01:
            print("Error : ", err_num01, "\n")
            continue

        num2 = input("Second Number >  ")
        try:
            num2 == int(num2)
        except Exception as err_num02:
            print("Error : ", err_num02, "\n")
            continue

    else:
        print("you are doing mistake")
        print("its a '[Calculator]' so type operator i.e. + - * / ** %")
        print("*" * 50)

    if int(num1) == 45 and int(num2) == 3 and ope_cal == "*":
        print("Result is '[555]' ")
    elif int(num1) == 56 and int(num2) == 9 and ope_cal == "+":
        print("Result is '[77]' ")
    elif int(num1) == 56 and int(num2) == 6 and ope_cal == "/":
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
        elif ope_cal == "**":
            print(num1 ** num2)
        elif ope_cal == "%":
            print(num1 / num2)
# End of the program
