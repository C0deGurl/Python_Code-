# Python_Code-HW # 1

Problem 0 – hello.py: Hello world! Write a program that always prints out Hello world! exactly (that’s 12 characters, including the space and the exclamation mark).

print("Hello world!")

Problem 1 – greet.py: Greeting Write a program that accepts one command line input value, and prints out the message Welcome, hargi! exactly, where hargi stands for whatever was entered as the command line input argument. Once again, make sure your output matches the required format. 

import sys

name = (sys.argv[1])
print("Welcome, " + name +"!")


Problem 2 – multiply.py: Multiplication. Write a program that reads two integer values x and y from the command line and prints their product (also an integer).

import sys

x = int(sys.argv[1])
y = int(sys.argv[2])

print(x*y)


Problem 3 – coins.py: US dollars to coins Write a program that reads a floating point dollar amount as a command line argument, and prints out the number of quarters (25c), dimes (10c), nickels (5c), and single cents. The output should consist of space-separated integers.

import sys 
dollar = round(float(sys.argv[1])* 100)

Quarters = dollar//25
dollar = dollar%25

Dimes = dollar//10
dollar = dollar%10

Nickels = dollar//5
dollar = dollar%5

Cents = dollar//1
dollar = dollar%1

print(Quarters,Dimes,Nickels,Cents)


Problem 4 – three_sort.py: Sort three numbers Write a program that takes three integer values a, b, and c from the command line and prints them in ascending order, separated by a space. You can use the built-in min() and max() functions.

import sys

n1 = int(sys.argv[1])
n2 = int(sys.argv[2])
n3 = int(sys.argv[3])

summed = n1 + n2 + n3
values = [n1,n2,n3]
biggest = max(values)
smallest = min (values)
in_between = summed - int(smallest) - int(biggest)
middle = str(in_between)
total = str(smallest)
sum = str(biggest)
print(total + " " + middle + " " + sum)
