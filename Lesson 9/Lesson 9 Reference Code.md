```python

# Draw Polygon
import turtle

sides_str = input("Please input the sides of a polygon: ")

sides = int(sides_str)

inner_angle = (sides - 2) * 180 / sides

turtle.penup()
turtle.setpos(-100, -100)
turtle.pendown()
turtle.color("red", "yellow")
turtle.pensize(2)

turtle.begin_fill()

for i in range(1, sides+1):
    turtle.forward(80)
    turtle.left(180 - inner_angle)

turtle.end_fill()



	
	
# Draw Rainbow
import turtle

colors = ["red", "purple", "blue", "green", "orange", "yellow"] 
turtle.bgcolor("black")

for i in range(200):
    color = colors[i%6]         # get the different color
    turtle.pencolor(color)      # change the pen color
    pen_size = i/50 + 1         # increase pen size by 1 after each 50 loops
    turtle.pensize(pen_size)    # change the pen size
    turtle.forward(i)           # move i steps
    turtle.left(59)             # turn 59 degrees anti-clockwise
	
	

# Draw Singapore Flag
import turtle

# singapore national flag Proportion:	3:2
flag_width = 450
flag_height = 300
radius = 55
star_length = 20

# move the pen to a position so we can draw the flag at the centre of the screen
turtle.penup()
turtle.setpos(-flag_width/2, 0)
turtle.pendown()

# draw a red rectangle filled with red color
turtle.color("red")
turtle.begin_fill()
for i in range(2):
    turtle.forward(flag_width)
    turtle.left(90)
    turtle.forward(flag_height/2)
    turtle.left(90)
turtle.end_fill()   # final direction: point left

# move the pen to the bottom-left corner
turtle.penup()
turtle.right(90)    # direction: point down
turtle.forward(flag_height/2)
turtle.pendown()
turtle.left(90)     # direction: point left

# draw a black border for the flag
turtle.color("black")
for i in range(2):
    turtle.forward(flag_width)
    turtle.left(90)
    turtle.forward(flag_height)
    turtle.left(90) # final direction: point left   

# move the pen to a new postion for drawing a circle
turtle.penup()
current_pos = turtle.pos()
turtle.setpos(current_pos[0]+100, current_pos[1]+170)
turtle.pendown()

# draw the first circle and filled with white color
turtle.color("white")
turtle.begin_fill()
turtle.circle(radius)   # direction: point left
turtle.end_fill()

# move the pen to a new position to draw another circle
turtle.penup()
turtle.forward(20)
turtle.pendown()

# draw the second circle and filled with red color
turtle.color("red")
turtle.begin_fill()
turtle.circle(radius)   # direction: point left
turtle.end_fill()

# move the pen to a new position for drawing the star (bottom-right star)
turtle.penup()
current_pos = turtle.pos()
turtle.setpos(current_pos[0]+10, current_pos[1]+30)
turtle.pendown()

# draw the 5 stars (first one will be the bottom-righ star)
turtle.color("white")
for i in range(1, 6):
    turtle.begin_fill()
    for j in range(5):
        turtle.forward(star_length)
        turtle.right(144)
    turtle.end_fill()

    turtle.penup()
    turtle.left(i*72)
    turtle.forward(35)
    turtle.right(i*72)
    turtle.pendown()

# move the pen back at the corner of flag
turtle.penup()
turtle.setpos(-flag_width/2, 0)


```
