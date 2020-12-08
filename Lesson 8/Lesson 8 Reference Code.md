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


