# Python_Code-

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
