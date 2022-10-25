#Write a program to accept a number from a user and calculate the sum of all numbers from 1 to a given number

#For example, if the user entered 10 the output should be 55 (1+2+3+4+5+6+7+8+9+10)

number_1 = int(input("Enter any number: "))
sum = 0
for i in range(1, number_1+1):
    print(f"{i},", end="")
    sum = sum + i # sum =+ i de yazılabilir..
print("\nTotal of the number : ", sum)


##Write a program to count the total number of digits in a number using a while loop.
number = int(input("Enter any number: "))
cnt = 0
while number != 0:
    cnt = cnt + 1
    a = number // 10
    number = a
print("Total digits are: ", cnt)


#Write a program to use for loop to print the following reverse number pattern
row = 5
k = 5
for i in range(0, row +1 ):
    for j in range(k-i, 0 , -1):
        print(j, end="")
    print()



#The Fibonacci Sequence is a series of numbers. The next number is found by adding up the two numbers before it. The first two numbers are 0 and 1.
#For example, 0, 1, 1, 2, 3, 5, 8, 13, 21. The next number in this series above is 13+21 = 34.
x = int(input("Enter any number: "))
num1 = 0
num2 = 1
for i in range(x):
    # print next number of a series
    print(num1, end=" ")
    # add last two numbers to get next number
    fs = num1 + num2
    # update values
    num1 = num2
    num2 = fs


#Write a program to use the loop to find the factorial of a given number.
#The factorial (symbol: !) means to multiply all whole numbers from the chosen number down to 1.

x = int(input("\nEnter the number that u want to calculate factorial: "))
fct = 1
if x < 0:
    print("factorial does not exist for negative numbers.")
elif x == 0:
    print("0! = 1")
else:
    for i in range(1, x+1):
        fct = fct * i
    print(f"{x}! = {fct}")




#Reverse a given integer number

x = int(input("Enter any number that u want to reserve: "))
rsv_n = 0
while x != 0:
    last_d = x % 10
    rsv_n = rsv_n * 10 + last_d
    x = x // 10
print(rsv_n)

##Write a program to calculate the sum of series up to n term. For example, if n =5 the series will become 2 + 22 + 222 + 2222 + 22222 = 24690
x = int(input("Enter any number: "))
twos = 2
sum = 0
for i in range(x):
    print(twos, end="+")
    sum = sum + twos
    twos = twos * 10 +2

print("\n Sum of above series is :", sum)