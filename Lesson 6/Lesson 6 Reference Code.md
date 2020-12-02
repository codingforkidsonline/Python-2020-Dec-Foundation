```python

s = "school"
print("s is:", s)

a = "school"[0]
print("a is:", a)

b = s[0]
print("b is:", b)



s = "school"
print("s is:", s)

a = "school"[1]
print("a is:", a)

b = s[1]
print("b is:", b)



# how to print out the last character in school?
s = "school"
last_character = s[5]
print(last_character)

# what happen if we print s[6]?
#print(s[6])



# another way to print out the last character of a string
s = "school"
last_character = s[-1]   # index -1 is pointed to the last character in a string
print(last_character)
print(s[-2])



# assign multiple linse of string to a variable
s = """National Day of Singapore is celebrated every year on August 9, 
in commemoration of Singapore's independence 
from Malaysia in 1965"""
print(s)



# connect two strings
s1 = "I want to go to "
s2 = "school"
print(s1)
print(s2)

t = s1 + s2
print(t)



# connect a string and a number
s1 = "I am "
age = 11
s2 = " years old"

#t = s1 + age + s2  # this will fail as you can't add string with number directly
t = s1 + str(age) + s2
print(t)



# duplicate strings
s = "school"
t = s * 3

print("s is:", s)
print("t is:", t)



# find a sub string
s = "I want to go to school"

sub1 = s[2:3]     # start from index 2: w   end before index 3: a 
print("sub1 is:", sub1)

sub2 = s[2:4]     # start from index 2: w   end before index 4: n 
print("sub2 is:", sub2)

# get the sub string of want
sub3 = s[2:6]
print("sub3 is", sub3)



s = "I want to go to school"

# get the sub string from beginning till go by omit the first index
sub4 = s[:12]
print("sub4 is:", sub4)

# get the sub string from go till end of the string by omit the second index
sub5 = s[10:]
print("sub5 is:", sub5)



# reverse a string
s = "School"
r = s[::-1]
print(r)



# make a string all upper case
s = "School"
us = s.upper()
print(us)



# make a string all lower case
s = "SingAporE"
ls = s.lower()
print(ls)



# find a index of a character
s = "school"
index1 = s.index("h")
index2 = s.index("o", )
print("index1 is:", index1)
print("index2 is:", index2)

# find the count of a character in a string
count1 = s.count("h")
count2 = s.count("o")
print("count1 is:", count1)
print("count2 is:", count2)



# find a index of a sub string
s = "I want to go to school"
index1 = s.index("want")
index2 = s.index("go")
print(index1)
print(index2)



# what happen if the characters are not found?
s = "I want to go to school"
index = s.index("home")   # we will learn how to handle the exception in the future lesson
print(index)



# use s.find() which has the same function as s.index, 
# but it returns -1 if the characters are not found
s = "I want to go to school"
index1 = s.find("school")
index2 = s.find("home")
print(index1)
print(index2)



# remove the whitespace at the beginning or end of the string
s = "   I want to go to school   "
print(s, "this message is after s")
t = s.strip()
print(t, "this message is after t")



# split a string based on space
s = "I want to go to school"
t = s.split()
print(t)



# slipt a string based on comma
s = "hello,my name is David,I am 11 years old"
t = s.split(",")
print(t)



# find the length of a string
s = "school"
print(len(s))



# compare two strings
s1 = "school"
s2 = "school"
print(s1 == s2)



# compare two strings
s1 = "school"
s2 = "School"
print(s1 == s2) # s and S are different



# print out each character of a string with for loop
s = "School"
for c in s:
  print(c)

  

# capture an input as a string
name = input("Please provide your name: ")
age = input("Please provide your age: ")
print("Hello " + name + ", I know your age is " + age)

```