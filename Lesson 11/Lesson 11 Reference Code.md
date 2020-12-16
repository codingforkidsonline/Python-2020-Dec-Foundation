
```python

# Version 10
# use randint() function to generate the initial position of the player

from random import randint

def print_winner_message():
  print("\nYou did it! Your mission is completed!")
  print("* * * * * * * * * * * * * * * * * * * * * * *")
  print("*            You are the WINNER!            *")
  print("* * * * * * * * * * * * * * * * * * * * * * *")


def print_gameover_message():
  print("\nYou lost the game!")
  print("* * * * * * * * * * * * * * * * * * * * * * *")
  print("*                GAME OVER!                 *")
  print("* * * * * * * * * * * * * * * * * * * * * * *")


def hit_wall():
  global current_health_point   #as we need to modify this global variable, we need to declare it as global
  current_health_point -= 1
  if current_health_point > 0:
    print(hit_wall_msg)
    print("Your remaining health point is", current_health_point)
    return "OK"
  else:
    print("You have used up all your health point!")  
    print_gameover_message()
    return "GAMEOVER"


def discover_letter():
  print(smart_move_msg)
  # below print statement is for debugging purpose, disable it when playing the game
  # print("current row: " + str(current_row), "current column: " + str(current_col))  
  if forest[current_row][current_col] != "":
    letter = forest[current_row][current_col]
    print("You have discovered a letter: " + letter)
    letter_list.append(letter)
    forest[current_row][current_col] = ""   # set this cell to empty as the letter is discovered  
  if len(letter_list) == word_length:
    print("\nCongratulation! You have discovered all the letters.")
    print(letter_list)
    print("\nYour final task is to guess the secret word.")
    guess = input("What is the secret word in your mind? ")
    if(guess.upper() == secret_word.upper()):
      print_winner_message()
      return "WIN"
    else:
      print("Wrong guess!")  
      print_gameover_message()
      return "LOSE"
  else:
    return "CONTINUE"


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
current_row = randint(0, map_row_count-1)  
current_col = randint(0, map_col_count-1)  
# for testing purpose only, comment out below print when playing the game
print("Player's initial position:", current_row, current_col) 

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
    if current_col == 0:      
      result = hit_wall()
      if(result == "GAMEOVER"):
        break;
    else:      
      current_col -= 1
      result = discover_letter()
      if(result == "WIN" or result == "LOSE"):
        # you might want to let the user to go to next level if they have won the current level
        break;
  elif response == "right" or response == "r":
    if current_col == map_col_count-1:      
      result = hit_wall()
      if(result == "GAMEOVER"):
        break;
    else:
      current_col += 1
      result = discover_letter()
      if(result == "WIN" or result == "LOSE"):
        break;
  elif response == "up" or response == "u":
    if current_row == 0:      
      result = hit_wall()
      if(result == "GAMEOVER"):
        break;
    else:
      current_row -= 1
      result = discover_letter()
      if(result == "WIN" or result == "LOSE"):
        break;
  elif response == "down" or response == "d":
    if current_row == map_row_count-1:      
      result = hit_wall()
      if(result == "GAMEOVER"):
        break;
    else:
      current_row += 1
      result = discover_letter()
      if(result == "WIN" or result == "LOSE"):
        break;
  elif response == "quit" or response == "exit":
    print("\nThanks for playing this game, bye-bye!")
    break;
  else:
    print("Invalid move, try again.")
	
```