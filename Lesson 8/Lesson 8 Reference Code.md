```python

# create a dictionary with key-value pair in {}
d = {
      "key1": "value1",
      "key2": 2,
      3: "value3"
    }
print(d)

print("the value of key key1 is:", d["key1"])
print("the value of key key2 is:", d["key2"])
print("the value of key 3 is:", d[3])



# change a value in a dictionary
student = {
            "name": "Sam",
            "age": 12
          }
print(student["age"])

student["age"] = 18
print(student["age"])



# add a new item (key-value pair) into a dictionary
colors = {
            "red": 1,
            "green": 2,
            "blue": 3
         }
print(colors)

colors["white"] = 4
print(colors)

# remove an item from the dictionary
colors.pop("blue")
print(colors)



# check if a key exists in a dictionary
colors = {
            "red": 1,
            "green": 2,
            "blue": 3
         }

if "green" in colors:
  print("we found green in colors")
else:
  print("we didn't find green in colors")
  
  

# print out all the keys in the dictionary
colors = {
            "red": 1,
            "green": 2,
            "blue": 3
         }

for key in colors:
  print(key)
  
  

# print out all the values in the dictionary
colors = {
            "red": 1,
            "green": 2,
            "blue": 3
         }

for value in colors.values():
  print(value)
  
  

# copy a dictionary
colors1 = {
            "red": 1,
            "green": 2,
            "blue": 3
         }

# colors2 = colors1 will not work for copy

colors2 = colors1.copy()
colors2["red"] = 0
print("colors1:", colors1)
print("colors2:", colors2)



# use dict() to create a copy of a dictionary
colors1 = {
            "red": 1,
            "green": 2,
            "blue": 3
         }

colors2 = dict(colors1)
colors2["red"] = 0
print("colors1:", colors1)
print("colors2:", colors2)



# check the how many items are in a dictionary
colors = {
            "red": 1,
            "green": 2,
            "blue": 3
         }
count = len(colors)
print(count)



# clear all the items in a dictionary
colors = {
            "red": 1,
            "green": 2,
            "blue": 3
         }
print("before clear:", colors)

colors.clear()
print("after clear:", colors)

count = len(colors)
print("the total items in colors is:", count)



# create a empty dictionary
d = {}
count = len(d)
print("the total items in this dictionary is:", count)


# Famous Scientists

# ******************
# * first approach *
# ******************
votes = ["Newton", "Einstein", "Gauss", "Darwin", "Gauss", "Euler", 
         "Pythagoras", "Newton", "Euler", "Darwin", "Einstein",
         "Edison", "Gauss", "Euler", "Newton", "Darwin", "Einstein",
         "Einstein", "Edison", "Einstein", "Gauss", "Galileo", "Einstein",
         "Gauss", "Galileo", "Newton", "Gauss"]

# create a empty dictionary
scientists = {}

# check the name one by one in the votes
for name in votes:
  if name not in scientists:
    scientists[name] = 1
  else:
    scientists[name] = scientists[name] + 1

# print out the survey result
print("the survey result:", scientists)

max_count = 0
for count in scientists.values():
  if count > max_count:
    max_count = count

print("max count is:", max_count)

# create a empty list to store the most famous scientists (might be more than 1)
mfs = []

for name in scientists:
  if scientists[name] == max_count:
    mfs.append(name)

print("most famous scientists are:", mfs)



```