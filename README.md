# assignment1-python-
#ques 1
print("""Twinkle, twinkle, little star,
\tHow I wonder what you are!
\t\tUp above the world so high,
\t\tLike a diamond in the sky.
Twinkle, twinkle, little star,
\tHow I wonder what you are""")


#ques2
first_name = input("Enter your first name: ")
last_name = input("Enter your last name: ")
print(last_name + " " + first_name)


#ques3
import math
radius = float(input("Enter the radius of the circle: "))
area = math.pi * (radius ** 2)
print("The area of the circle with radius", radius, "is:", area)

#ques 4
color_list = ["Red","Green","White","Black"]
print("First color:", color_list[0])
print("Last color:", color_list[-1])

#ques5
n = input("Enter an integer: ")
n1 = int(n)
n2 = int(n * 2)   # 'nn'
n3 = int(n * 3)   # 'nnn'
result = n1 + n2 + n3
print("Result of n+nn+nnn is:", result)


#ques6
numbers = input("Enter comma-separated numbers: ")
number_list = numbers.split(",")
number_tuple = tuple(number_list)
print("List:", number_list)
print("Tuple:", number_tuple)

#ques7
celsius = float(input("Enter temperature in Celsius: "))
fahrenheit = (celsius * 9/5) + 32
print(f"{celsius}°C is equal to {fahrenheit}°F")

#ques8
a = int(input("Enter first number: "))
b = int(input("Enter second number: "))
print(f"Before swapping: a = {a}, b = {b}")
a, b = b, a
a += 1
print(f"After swapping and incrementing 'a': a = {a}, b = {b}")


#ques9
num = int(input("Enter a number: "))

if num % 2 == 0:
    print(num, "is Even")
else:
    print(num, "is Odd")

#ques10
year = int(input("Enter a year: "))

if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):
    print(year, "is a Leap Year")
else:
    print(year, "is not a Leap Year")


#ques 12
import math
x1, y1 = map(float, input("Enter coordinates of first point (x1 y1): ").split())
x2, y2 = map(float, input("Enter coordinates of second point (x2 y2): ").split())
distance = math.sqrt((x2 - x1) ** 2 + (y2 - y1) ** 2)
print("Euclidean Distance:", distance)


#ques11
year = int(input("Enter a year: "))

if (year % 400 == 0) or (year % 4 == 0 and year % 100 != 0):
    print(year, "is a Leap Year")
else:
    print(year, "is not a Leap Year")


#ques13
a = float(input("Enter first angle: "))
b = float(input("Enter second angle: "))
c = float(input("Enter third angle: "))
if a + b + c == 180 and a > 0 and b > 0 and c > 0:
    print("The angles form a triangle")
else:
    print("The angles do not form a triangle")


#ques 14
P = float(input("Enter principal amount: "))
R = float(input("Enter annual interest rate (%): "))
T = float(input("Enter time (years): "))
A = P * ((1 + R / 100) ** T)
CI = A - P
print("Compound Interest:", CI)
print("Total Amount:", A)


#ques 15
n = int(input("Enter a positive integer: "))

if n > 1:
    for i in range(2, int(n**0.5) + 1):
        if n % i == 0:
            print(n, "is not a Prime Number")
            break
    else:
        print(n, "is a Prime Number")
else:
    print("Number must be greater than 1")

    
#ques16
N = int(input("Enter a positive integer: "))
sum_of_squares = sum(i**2 for i in range(1, N+1))
print("Sum of squares up to", N, "is:", sum_of_squares)
    
