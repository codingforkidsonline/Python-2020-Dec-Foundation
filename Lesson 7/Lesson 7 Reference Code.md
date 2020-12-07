```python

# define a variable and assign a list of numbers to it
numbers = [1, 5, 2, 99, 10]
print(numbers)



# define a variable and assign a list of strings to it
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
print(week_days)



# you can even put the numbers and strings into the same list
mixed_list = [1, 5, 2, "Mon", "Fri"]
print(mixed_list)



# use index to access the item in the list
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]

first_day = week_days[0]  # index starts from 0, index 0 is pointing to the first item in the list
second_day = week_days[1]
seventh_day = week_days[6]

print("first weekday is: ", first_day)
print("second weekday is: ", second_day)
print("seventh weekday is: ", seventh_day)

# what happen if you want to get the eighth weekday?
#eighth_day = week_days[7]



# access the range of the list
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
print(week_days[1:4])  # from index 1 to the item before index 4



# access from the beginning of the list till Saturday
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
print(week_days[:6])



# access from the Wednesday till end of the list
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
print(week_days[2:])



# access the last item in the list
numbers = [1, 5, 2, 99, 10]

last_number = numbers[4]
print(last_number)

last_number = numbers[-1]
print(last_number)

# access the second last item in the list
second_last_number = numbers[-2]
print("second last number is:", second_last_number)



# change the value in the list
numbers = [1, 5, 2, 99, 10]
print("before the change:", numbers)

numbers[1] = 0  # we are changing the second number
print("after the change:", numbers)



# loop through the list
numbers = [1, 5, 2, 99, 10]
sum = 0
for n in numbers:
  sum = sum + n

print("the sum of all the numbers in the list is:", sum)



# check if an item exists in the list
numbers = [1, 5, 2, 99, 10]

if 99 in numbers:
  print("we found 99 in the list")
else:
  print("we didn't find 99 in the list")

if 100 in numbers:
  print("we found 100 in the list")
else:
  print("we didn't find 100 in the list")
  
  

# add an item to the end of the list
numbers = [1, 5, 2, 99, 10]
numbers.append(100)
print(numbers)



# insert an item to a specific position in the list
numbers = [1, 5, 7, 99, 10]
numbers.insert(2, 88) # insert 88 into index position 2, the original number at index position 2 will be pushed back
print("after insert 88:", numbers)

# remove 88 from the list
numbers.remove(88)
print("after remove 88:", numbers)

# remove the last item in the list
numbers.pop()
print("after remove the last item:", numbers)

# remove the item based on the given index
numbers.pop(2)
print("after remove 7:", numbers)

# remove all the items in the list
numbers.clear()
print("after remove all the items:", numbers)



# try to copy a list
number_list1 = [1, 5, 2, 99, 10]
number_list2 = number_list1

# change a value in numberList2
number_list2[0] = 100

# we can see the first item in both lists are changed
# this is because numberList2 is just a reference of numberList1
print("number list 1 is:", number_list1)
print("number list 2 is:", number_list2)



# to create a separate copy from numberList1
number_list1 = [1, 5, 2, 99, 10]
number_list2 = number_list1.copy()
number_list2[0] = 100
print("number list 1 is:", number_list1)
print("number list 2 is:", number_list2)



# use list() to create a separate copy from numberList1
number_list1 = [1, 5, 2, 99, 10]
number_list2 = list(number_list1)
number_list2[0] = 100
print("number list 1 is:", number_list1)
print("number list 2 is:", number_list2)



# join two lists
list1 = ["a", "b" , "c"]
list2 = [1, 2, 3, 3.8]
joined_list = list1 + list2
print(joined_list)



# sort the list
number_list1 = [1, 5, 2, 99, 10]
print("before sort:", number_list1)

number_list1.sort()
print("after sort:", number_list1)



# descending sort
number_list2 = [1, 5, 2, 99, 10]
number_list2.sort(reverse = True)
print("after descending sort:", number_list2)



# sort the list of strings
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
week_days.sort()
print(week_days)



# calculate how many items are in a list
week_days = ["Mon", "Tue", "Wed", "Thu", "Fri", "Sat", "Sun"]
count = len(week_days)
print(count)



# create a empty list
empty_list = []
print(empty_list)

count = len(empty_list)
print("the total items in this list is:", count)



# use input() to capture 4 numbers and put them into a number list
# print out the number list and the biggest the number in the list

number_list = []
for i in range(4):
  number_str = input("Please input a number: ")
  number = int(number_str)  # what happen if you do not have this line of code?
  number_list.append(number)

print(number_list)

number_list.sort()
max_number = number_list[-1]
print(max_number)



# a list inside a list
big_list = [
              [1, 2, 3],
              [4, 5, 6] 
          ]
print("big list:", big_list)
print("first row in big list:", big_list[0])
print("second row in big list:", big_list[1], "\n")

print("first row, first column:", big_list[0][0])
print("first row, second column:", big_list[0][1])
print("first row, third column:", big_list[0][2], "\n")

print("second row, first column:", big_list[1][0])
print("second row, second column:", big_list[1][1])
print("second row, third column:", big_list[1][2], "\n")

# change the value of second row and third column to 100
big_list[1][2] = 100
print(big_list)



# draw a star with for loop and located at the centre of the screen
import turtle

turtle.color("blue")

turtle.begin_fill()

# try to position our star at the centre of the screen
turtle.penup()
turtle.setpos(-125, 50)
turtle.pendown()

for i in range(5):
    turtle.forward(250)
    turtle.right(144)

turtle.end_fill()


```