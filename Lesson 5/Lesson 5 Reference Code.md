```python

print(2>1 and 3 > 1)
print(2>1 and 1 > 3)

print(2>1 or 3>1)
print(2>1 or 1>3)

print(not 2>1)
print(not 1>3)



# try to change the value of number and see what different message is printed out
# always put colon (:) at the end of each if/elif/else statement
number = 3
if number > 3:
  print("the value of number is:", number)
  print("the number is greater than 3")    
elif number < 3:
  print("the value of number is:", number)
  print("the number is less than 3")
else:
  print("the value of number is:", number)
  print("the number is same as 3")

  
  
# example of wrong indent
a = 1
b = 2
  c = a + b
print(c)



# example of wrong indent in if statement
a = 10
if a > 9:
print("a is greater than 9")



# Print i as long as i is less than 5
# take note the indent in the while loop statement
# try to see what happens if you remove the indent for print(i)
# try to see what happens if you remove the indent for i = i + 1
i = 0
while i < 5:
  print(i)
  i = i + 1
print("the while loop is completed")



# try another way to do i = i + 1
i = 0
while i < 5:
  print(i)
  i += 1  # same as i = i + 1
print("the while loop is completed")



# break statement in while loop: allow us to stop the while loop even if the while condition is true
i = 0
while i < 5:
  print(i)
  if i == 3: 
    break
  i = i + 1
print("the while loop is completed")



# else statement in while loop: 
# allow us to run a block of code once when the condition is no longer true
i = 0
while i < 5:
  print(i)
  i = i + 1
else:
  print("i is now equal to 5")
print("the while loop is completed")



number_list = range(0, 10)
print(list(number_list))

number_list = range(10)
print(list(number_list))

number_list = range(3, 10)
print(list(number_list))



# The range() function defaults to increment the sequence by 1, 
# it is possible to specify the increment value by adding a third parameter
number_list = range(0, 10, 2)  # increase each number by 2
print(list(number_list))

number_list = range(1, 10, 2)  # increase each number by 2
print(list(number_list))




for x in range(10):
  print(x)          # take note that the x stops at 9

  
  
# break statement
for x in range(10):
  print(x)   
  if x == 5:
    break

	
	
# continue statement
for x in range(10):
  if x == 5:
    continue  # check if you have 5 in your output
  print(x)

  
  
# else statement in for loop: 
# allow us to run a block of code once when the loop is finished
for x in range(10):
  print(x)
else:
  print("the loop is finished")

  
  
# use for loop to print out a 5x5 square of #
for i in range(5):
  print("# " * 5)

  
  
# use for loop to print out a square of # with border only
for i in range(5):
  if i == 0 or i == 4:  # use or operator, it will return True as long as one expression is true
    print("# " * 5)     # one line has 9 characters
  else:
    print("#       #")  # need 7 spaces

	

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
turtle.left(90)

	
	
# draw a colorful square with for loop	
import turtle

turtle.pensize(3)

my_colors = ["red", "blue", "purple", "orange"]

for i in range(4):
    my_line_color = my_colors[i]
    turtle.color(my_line_color)
    turtle.forward(200)
    turtle.left(90)
	

# draw a colorful and differnt pensize square with for loop	
import turtle

color_list = ["red", "blue", "purple", "orange"]
pensize_list = [2, 4, 6, 10]

for i in range(4):
    line_color = color_list[i]
    turtle.color(line_color)
    line_pensize = pensize_list[i]
    turtle.pensize(line_pensize)
    turtle.forward(200)
    turtle.left(90)

```