```python

# Question 1 Ansower:
d = {1:20, 2:20, 4:40}
print("before add:", d)

d[3] = 30
print("after add:", d)



# Question 2 Ansower:
n_str = input("Please input a number: ")

# n = ?

n = int(n_str)

d = {}
for i in range(1, n+1):
  d[i] = i ** 2

print(d)



# Question 3 Ansower:
d = {1:12, 2:33, 3:4, 4:52, 5:17}

sum = 0
for i in d.values():
  sum += i

print(sum)



# Question 4 Ansower:
* use the value in list1 as the key
* use the value in list2 as the value
* there are 9 items in both lists
* print out the dictionary
"""

list1 = [1, 2, 3, 4, 5, 6, 7, 8, 9]
list2 = [1, 4, 9, 16, 25, 36, 49, 64, 81]

d = {}

for i in range(9):
  key = list1[i]
  value = list2[i]
  d[key] = value

print(d)



# Question 5 Ansower:
d = {
      "name1": "David Law",
      "name2": "Lee Ming Yang",
      "name3": "Frack Tan",
      "name4": "Eric Wong"
    }

d["name2"] = "Liu Laoshi"

for key in d:
  if key == "name2":
    print(d[key])
    break


	
# Question 6 Ansower:
fruits = {
            "apple": 4,
            "orange": 2,
            "pear": 5,
            "watermallon": 10
        }

sum = 0
for key in fruits:
  print(key, fruits[key], sep=":")
  sum += fruits[key]

print("the total sum is:", sum)



# Question 7 Ansower:
  > for example, as number 3 appears 2 times in the list, you can store the key:value pair as 3:2 in the dictionary
"""

number_list = [3, 27, 4, 5, 21, 3, 19, 27, 4, 11, 27, 19]

d = {}

for n in number_list:
  if n not in d:
    d[n] = 1
  else:
    d[n] += 1

print(d)



# Question 8 Ansower:
d = {
      "Germany": "Berlin",
      "India": "New Delhi",
      "Italy": "Rome"
    }

d.clear()
d["China"] = "Beijing"
d["Canada"] = "Ottawa"
d["Italy"] = "Rome"

print(d)



```
