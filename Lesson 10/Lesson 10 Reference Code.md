```python

# we can use dir() function to list all the function names 
# and vairable names in a module

import math

dir(math)



# use random module to generate a random number

import random

# generate a random between 0.0 to 1.0
r = random.random()
print(r)



# only import randint() function from random module

from random import randint

# generate a random integer from 1 to 100
r = randint(1, 100)
print(r)



# use datetime class in datetime module to 
# diplay the current date time (UTC time)

from datetime import datetime

current_time = datetime.now()
print(current_time)



# define a function to calculate the average value of two numbers
def average(a, b):
  sum = a + b
  ave = sum/2
  return ave

# call the function 1st time
result1 = average(1, 2)
print("result 1 is:", result1)

# call the function 2nd time
result2 = average(10, 20)
print("result 2 is:", result2)



# Secret Message
sentence = input("Assume you are Greg the Dog, please write a sentence to Sam the Cat with your secret message: ")
word_list = sentence.split()
print(word_list)
secret_message = ""
for w in word_list:
  secret_message = secret_message + w[0]
print("The secret message deciphered is:", secret_message)



# Crazy Dog
sentence = input("Please input a sentence: ")
number_of_e = 0
for c in sentence:
  if c == "e" or c == "E":
    number_of_e += 1  # you can also use: number_of_e = number_of_e + 1

if number_of_e == 0:
  print("happy")
elif number_of_e <= 3:
  print("sad")
else:
  print("CRAZY!")
  
  
  
# Dog Treats
a = 1
b = 1

treats = []
treats.append(a)
treats.append(b)

for i in range(3, 21):
  f = a + b
  treats.append(f)
  a = b
  b = f

print(treats)

count = len(treats)
print("the total numbers in the list is:", count)



# Bag of Bones
number_str = input("Please input the number of bones in the bag: ")
number = int(number_str)

if number<2 or number>100:
  print("Invalid number")
else:
  possible = False
  for i in range(2, number):
    if number % i == 0:
      possible = True
      break
  if possible:
    print("Yes")
  else:
    print("No")


```
