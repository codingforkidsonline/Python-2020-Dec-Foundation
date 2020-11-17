```python

# we have learned how to add numbers in Python
a = 10
b = 20
c = 30
sum = a + b + c
print("The sum of a, b and c is:", sum)



# subtruct a number
a = 20
b = 12
diff = a - b
print("The difference between a and b is:", diff)



# multiple numbers
a = 6
b = 7
product = a * b
print("The product of a and b is:", product)



# divide a number, the result would be a floating number (with decimal point)
a = 72
b = 8
quotient = a / b
print("The quotient of a is divided by b is:", quotient)

# what happen if it is not a perfect division?
m = 10
n = 3
quotient = 10 / 3
print("The quotient of m is divided by n is:", quotient)



# truncated division (floor division)
a = 17
b = 3
quotient = a / b
floor_result = a // b
print("The quotient of a is divided by b is:", quotient)
print("The integer part of the result of a is divided by b is:", floor_result)



# find the remainer 
a = 44
b = 6
remainder = a % b
print("The remainder of a is divided by b is:", remainder)



# find the square number
a = 11
square_number1 = a * a
print("The square of a is:", square_number1)
square_number2 = a ** 2
print("The square of a is:", square_number2)

b = 5
power1 = b * b * b
print("b to the power of 3 is:", power1)
power2 = b ** 3
print("b to the power of 3 is:", power2)



# mixed operation
result = 10 + 7 * 3 / (3+4) - 5
print(result)



# The power has higher priority than multiplication
result = 2 * 3 ** 2
print(result)



# let's compare the two values
print(10 < 20)
print(10 > 20)
print(10 == 20)
print(10 != 20)



# let's compare the two values
a = 10
b = 20
result1 = a < b
result2 = a > b
result3 = a == b
result4 = a != b
print("result1 is:", result1)
print("result2 is:", result2)
print("result3 is:", result3)
print("result4 is:", result4)



print(10 == 10)
print(10 != 10)

# try to uncomment and run the below code to see what error you will encounter
#print(10 = 10)



# Besides comparing the numbers, you can compare if the two strings are same
s1 = "Morning"
s2 = "Night"
print("Morning is same as night:", s1 == s2)
print("Morning is same as morning:", s1 == "morning")
print("Morning is same as Morning:", s1 == "Morning")



# calculate the area of a circle
r = 5
area = 3.14 * r ** 2
print("The area of a circle with radius 5 is:", area)



# calculate the area of a circle with pi
import math
print("The value PI is:", math.pi)

r = 5
area = math.pi * r ** 2
print("The area of a circle with radius 5 is:", area)



# calculate a square root of a given number
import math
a = 81
square_root1 = math.sqrt(a)
print("The square root of a is:", square_root1)

b = 80
square_root2 = math.sqrt(b)
print("The square root of b is:", square_root2)



# calculate greatest common divisor (GCD) 
import math
gcd1 = math.gcd(12, 16)
print(gcd1)

gcd2 = math.gcd(45, 60)
print(gcd2)



# You can do power calculation with ** operator 
power1 = 4 ** 2
power2 = 4 ** 3
print(power1)
print(power2)

# print a horizontal line
print("-" * 20)



# you can also do power calculation with math.pow
import math
power3 = math.pow(4, 2)
power4 = math.pow(4, 3)
print(power3)
print(power4)



# Factorials are used in finding permutations or combinations. 
# You can determine the factorial of a number by multiplying 
# all whole numbers from the chosen number down to 1.

# Let's calculate 7!
f1 = 7 * 6 * 5 * 4 * 3 * 2 * 1
print(f1)

import math
f2 = math.factorial(7)
print(f2)

# please do not try to calculate 100!. If you do it ...
f3 = math.factorial(100)
print(f3)


# draw a circle
import turtle

turtle.color("red")
turtle.pensize(5)
turtle.circle(100)




# draw a square
import turtle

turtle.color("red")
turtle.pensize(3)

turtle.forward(200)
turtle.left(90)

turtle.forward(200)
turtle.left(90)

turtle.forward(200)
turtle.left(90)

turtle.forward(200)



```