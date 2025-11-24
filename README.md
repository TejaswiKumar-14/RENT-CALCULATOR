# Room/Flat Expense Splitter

This Python script helps you calculate how much each person in a shared room/flat needs to pay based on monthly expenses such as rent, food, and electricity.


# Overview

Managing shared expenses can be confusing. This program takes the total monthly costs and divides them equally among all the people living in the room/flat.

You only need to input:

Monthly rent

Food expenses

Electricity usage (units consumed)

Electricity cost per unit

Number of people sharing the accommodation


The program then calculates:

Total electricity bill

Total monthly expense

Amount each person must pay


# How It Works

1. The user enters:

Rent amount

Total food expenses

Total electricity units consumed

Cost per electricity unit

Number of persons



2. The script calculates:

total_bill = electricity_spend * charge_per_unit
output = (food + rent + total_bill) // persons


3. It prints the split amount per person.



# Example Input/Output

Input:

Enter your hostel/flat rent = 6000
Enter the amount of food ordered = 3000
Enter the total of electricity spend = 150
Enter the charge per unit = 8
Enter the number of persons living in room/flat = 3

Output:

Each person will pay =  3400


# Features

Easy to use

Simple and clean code

Automatically calculates shared expenses

Prevents confusion in rent and bill splitting


# Code

rent = int(input("Enter your hostel/flat rent = "))
food = int(input("Enter the amount of food ordered = "))
electricity_spend = int(input("Enter the total of electricity spend = "))
charge_per_unit = int(input("Enter the charge per unit = "))
persons = int(input("Enter the number of persons living in room/flat = "))

total_bill = electricity_spend * charge_per_unit

output = (food + rent + total_bill) // persons

print("Each person will pay = ", output)
