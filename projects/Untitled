import os


def clear_screen():
    os.system("cls" if os.name == "nt" else "clear")


def projection_sales():
    clear_screen()
    sales = (covers * average_check) * hours_in_op
    hourly_sales(sales, hours_in_op)
    return sales

def hourly_sales(sales, hours_in_op):
    hourly = (sales / hours_in_op)
    return hourly


user = input("Please enter your name:   ")
covers = int(input("Hello Chef {}, How many covers per hour do you plan on seating?   ".format(user)))
average_check = int(input("Ok Chef {}, what do you want/think your check average will be?   ".format(user)))
hours_in_op = int(input("How many hours will you be in operation today?   "))


sales = projection_sales()


print("You are on track to have ${} in sales today.".format(sales))
print("You are projected to make ${} per hour.".format(hourly_sales(sales, hours_in_op)))



continue_to_food_cost = input("Would you like to know your food cost for the day?   ")


if continue_to_food_cost.upper() == "YES":
    print("OK")
