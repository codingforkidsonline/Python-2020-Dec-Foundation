```python

# Question 1 Answer:
flower_list = ["Tulip", "Sunflower", "Bluebell", "Rose", "Cherry blossom", "Orchid", "Lily"]

first_flower = flower_list[0]
fourth_flower = flower_list[3]
last_flower = flower_list[-1]

print(first_flower, fourth_flower, last_flower, sep=",")



# Question 2 Answer:
numbers = [21, 34, 59, 78, 6, 100]

sum = 0
for n in numbers:
  sum += n

print(sum)



# Question 3 Answer:
sentence = "You make a difference in my life"
word_list = sentence.split()
sub_list = word_list[2:]
print(sub_list)



# Question 4 Answer:
number_list = [3, 92, 5, 10, 17, 101, 24, 55]
odd_list = []

for n in number_list:
  if n % 2 != 0:
    odd_list.append(n)

print(odd_list)



# Question 5 Answer:
number_list = [3, 92, 5, 10, 17, 101, 24, 55]

length = len(number_list)

for i in range(length):
  if number_list[i] % 2 != 0:
    number_list[i] = number_list[i] + 1

print(number_list)



# Question 6 Answer:
number_list = []
for i in range(5):
  number_str = input("Please input your number: ")
  number = int(number_str)
  number_list.append(number)
print(number_list)

sum = 0
for n in number_list:
  sum += n

print("the sum is:", sum)



# Question 7 Answer:
number_list = [34, 42, 57, 21, 49, 91, 33, 19, 87]

number_list.sort()
smallest_number = number_list[0]
biggest_number = number_list[-1]
sum = smallest_number + biggest_number
print(sum)



# Question 8 Answer:
import turtle

turtle.color("red")
turtle.pensize(4)

for i in range(4):
    turtle.forward(100)
    turtle.left(90)

turtle.color("blue")
turtle.pensize(6)

turtle.penup()
turtle.setpos(-20, -20)
turtle.pendown()

for i in range(4):
    turtle.forward(140)
    turtle.left(90)


```
