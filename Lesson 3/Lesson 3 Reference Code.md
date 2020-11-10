## Python Identifiers
* Python Identifiers are used to define the name of varibles, function, class, structure, etc.
* Identifiers can be a combination of letters in lowercase (a to z) or uppercase (A to Z) or digits (0 to 9) or an underscore (_). Names like myClass, var_1 and print_this_to_screen, all are valid identifiers.
* Space is not allowed in an identifier
* A variable name must start with a letter or the underscore character. An identifier cannot start with a digit. 1variable is invalid, but variable1 and &nbsp;_1variable is perfectly fine.
* Keywords (like if, else, True) cannot be used as identifiers.
* Special symbols (like !, @, #, $, % etc.) cannot be used as identifiers.
* Do not use Python built-in data types (int, float, str, range, list, dict) as identifier
* Python is a case-sensitive language. This means, Count and count are completely different

```python

# this is the first comment, we write it for our own understanding, not for the computer
# this is the second comment


# the next line is the code to instruct the computer to print out something
print("It's a nice day!")


"""this is the first line of my comment
this is the second line of my comment
this is the third line of my comment"""



# let's practice how to use Python Identifiers

# a1 is a correct identifier
a1 = 1 
print(a1)


# 1a is not a correct identifier, if you run the code, you will see "invalid syntax" error message
#1a = 1 


# _ can be used as the first charactor of the variable
#_1a = 2
#print(_1a)




# assign variable x with a integer value 5
x = 5
print(x)

# assign variable y with a floating number 3.2 (a number with a decimal point)
y = 3.2
print(y)

# assign variable z with a string value "Stay Home! Stay Safe!"
z = "Stay Home! Stay Safe!"
print(z)



# assign variable x with a integer value 5
x = 5
print(x)

# overwrite variable x with a floating number 3.2 (a number with a decimal point)
x = 3.2
print(x)

# overwrite variable x with a string value "Stay Home! Stay Safe!"
x = "Stay Home! Stay Safe!"
print(x)






# assign the three variables in a single line (separated by ;)
x = 5; y = 3.2; z = "Stay Home! Stay Safe!"
print(x)
print(y)
print(z)

# print a horizontal line
print("--------------------------------")

# assign three variables with the same value
x = y = z = 100
print(x)
print(y)
print(z)




# sequence of assignment is important
print(t)
t = 10



# name of variable should be meaningful

# bad names 
a = 11
b = 150

# good names (use _ to separate words in your variable)
my_age = 11
my_height = 150



# name of varialbe is case sensitive
my_age = 11
print(my_Age)



# this is a single line statement
a = 1 + 2 + 3

# this is another single line statement
b = 4 + 5 + 6

print(a)
print(b)



# put multiple statements into a single line (separated by ;)
a = 1 + 2 + 3; b = 4 + 5 + 6

print(a)
print(b)



# put a single statement in two lines with \
a = 1 + 2 \
    + 3 + 4

print(a)



# a statement can have a variable as long as the variable has a given value
x = 10
y = 3 + x * 2
print(y)



# but the value of the variable must have the same data type as others in the statement
x = "Hello"
y = 3 + x * 2
print(y)



# print a message on the screen
print("I am going to print this sentence on my computer screen!")

# print a number on the screen
print(5)

# print a variable on the screen
x = 10
print(x)



# connect two strings together and print it out
a = "I am"
b = "Liu Laoshi"

print(a + b)
print (a + " " + b)



# connect two strings together as another string and print it out
a = "I am"
b = "Liu Laoshi"
c = a + b
d = a + " " + b
print(c)
print(d)



# we know how to print out the integer and the string separately,
# what if we want to print them together to make our printed output more meaningful?
a = 5
b = 6
sum = a + b
print(sum)
print("the sum of a + b is:", sum)




# format a long output message
my_name = "Daniel"
my_age = 13
print("My name is", my_name, "and I am", my_age, "years old" )




# a better way to format a long output message
my_name = "Daniel"
my_age = 13
print("My name is {0} and I am {1} years old".format(my_name, my_age))




# Practie: how to print out the below message by using the given varibles?
# Message: My favorite flower is rose and my favorite food is chicken rice
favorite_color = "red"
favorite_food = "chickent rice"
print("My favorite flower is {0} and my favorite food is {1}".format(favorite_color, favorite_food))



# print three numbers on the screen (the numbers are separated by a space)
x = 10; y = 20; z = 30
print(x, y, z)

# print three numbers on the screen (the numbers are separated by a *)
print(x, y, z, sep="*")

# print three numbers on the screen (the numbers are separated by a -)
print(x, y, z, sep="-")




# compare the two printed contents and explain why the outputs are different
a = "I love "
b = "Home-Based Learning"
print(a + b)
print(a, b)




# print some space in a message on the screen
print("this is the first line")
print(" this is the second line")
print("  this is the thrid line")
print("   this is the fourth line")
print("    this is the fifth line")




# print a horizontal continuous line
print("________________________________")

# print a horizontal doted line
print("--------------------------------")

# print a horizontal * line
print("********************************")

# print three empty lines (each \n give you one empty line)
print("\n\n\n")

# print a message after the empty lines
print("I am the message after the empty lines")




# let's have some fun by printing a diamond on the screen
print("     *")
print("    * *")
print("   *   *")
print("  *     *")
print(" *       *")
print("*         *")
print(" *       *")
print("  *     *")
print("   *   *")
print("    * *")
print("     *")




# let's print a number 7 on the screen
print("****************")
print("              *")
print("             *")
print("            *")
print("           *")
print("          *")
print("         *")
print("        *")
print("       *")



# Practice: how to print out a right triangle


```

