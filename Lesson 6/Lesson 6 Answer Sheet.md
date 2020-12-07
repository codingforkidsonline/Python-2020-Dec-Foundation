```python

# Question 1 Answer:
s = "Singapore's national day is on 9th August"
print("the 36th character is:", s[35])
print("the last character is:", s[-1])



# Question 2 Answer:
message1 = "Woodgrove Primary School"
message2 = " has more than "
message3 = 1000
message4 = " students"

sentence = message1 + message2 + str(message3) + message4
print(sentence)



# Question 3 Answer:
sentence = "Do You Want to Build a Snowman"
word_list = sentence.split()
last_word = word_list[-1]
print("before case change:", last_word)
changed_word = last_word.upper()
print("after case change:", changed_word)


# Question 4 Answer:
s = input("Please input a message: ")
print("before duplication:", len(s))

s = s * 2
print("after duplication:", len(s))



# Question 5 Answer:
sentence = "All the schools will be re-opened on 2 June in Singapore"
index = sentence.find("on")
print("the index of on is at:", index)

sub_sentence = sentence[:index]
print(sub_sentence)


# Question 6 Answer:
family_name = input("Please input your family name: ")
given_name = input("Please input your given name: ")

full_name = family_name + " " + given_name
print("Hello " + full_name)



# Question 7 Answer:
message = input("Please input a message: ")
if(len(message) > 15):
  print("enough characters")
else:
  print("not enough characters")



# Question 8 Answer:
import turtle

turtle.color("blue")
turtle.pensize(3)

turtle.begin_fill()
for i in range(3):
    turtle.forward(200)
    turtle.left(120)
turtle.end_fill()


```
