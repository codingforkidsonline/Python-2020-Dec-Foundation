```python

# Version 4:
# Start the game

# 1. your game title
print("* * * * * * * * * * * * * * * * * * * * * * *")
print("*                                           *")
print("*                 Word Hunt!                *")
print("*           Created By: Frank Wong          *")
print("*                                           *")
print("* * * * * * * * * * * * * * * * * * * * * * *")


# 2. game configuration data (global varibles)
# 2.1 define your secret word
secret_word = "GREAT" 
word_length = len(secret_word)

#2.2 define the forest map with n rows and m columns
forest = [
            ["A", "", "", "", ""],   # row 0
            ["", "G", "", "", ""],   # row 1
            ["", "", "R", "", ""],   # row 2
            ["E", "", "", "", ""],   # row 3
            ["", "", "", "", ""],    # row 4
            ["", "", "", "", "T"]    # row 5
        ]
map_row_count = len(forest)
map_col_count = len(forest[0])
# for testing purpose only, comment out below print when playing the game
print("map rows: {0}, map columns: {1}".format(map_row_count, map_col_count))


# 2.3 set the player's initial position in the forest
current_row = 0  #we can use randint()
current_col = 0  #we can use randint()

# 2.4 create a list to store the letters has been discovered by the player so far
letter_list = []

# 2.5 define what message to show to the user when the user hits a wall or makes a smart move
hit_wall_msg = "You are heading to a wall! Please try again."
smart_move_msg = "Smart move!"

# 2.6 set the level and health point info
level = 1
max_health_point = level*5+5   # auto adjust your death_hit based on the level
current_health_point = max_health_point     #health point is reduced by 1 after 1 wall hit


# 3. game guide
name = input("Please input your name before playing the Word Hunt game: ")
print("Hello " + name + ", you are in a dark forest now.\n")
print("Your mission is to hunt for a secret word with " + str(word_length) + " magic letters,")
print("and re-arrange the letters to discover the secret word.")
print("You can move around in the dark forest by typing left/right/up/down.")
print("You can quit the game by typing quit/exit.")
print("You are currently in level", level)
print("The hunting advanture is starting now...")


# 4. start the game
response = ""
while True:
  response = input("\nWhich direction would you like to move to? [left], [right], [up], [down]: ")
  if response == "left" or response == "l":
    print("move to left")  # we need to decide what to do if the user want to move to left
  elif response == "right" or response == "r":
    print("move to right")  # we need to decide what to do if the user want to move to rigth
  elif response == "up" or response == "u":
    print("move up")  # we need to decide what to do if the user want to move up
  elif response == "down" or response == "d":
    print("move down")  # we need to decide what to do if the user want to move down
  elif response == "quit" or response == "exit":
    print("\nThanks for playing this game, bye-bye!")
    break;
  else:
    print("Invalid move, try again.")



```
