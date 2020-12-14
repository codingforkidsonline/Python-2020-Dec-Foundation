```python

# Question 1 Answer:
import turtle

sides = 8

inner_angle = (sides - 2) * 180 / sides

turtle.penup()
turtle.setpos(-100, -100)
turtle.pendown()
turtle.color("black", "yellow")
turtle.pensize(2)

turtle.begin_fill()

for i in range(1, sides+1):
    turtle.forward(80)
    turtle.left(180 - inner_angle)

turtle.end_fill()



# Question 2 Answer:
import turtle

turtle.color("red")
turtle.pensize(2)

radius = 100
turtle.circle(radius)

turtle.penup()
turtle.backward(radius)
turtle.pendown()

for i in range(4):
    turtle.forward(radius*2)
    turtle.left(90)



# Question 3 Answer:
import turtle

turtle.color("red")
turtle.pensize(2)
side_length = 100

turtle.forward(side_length)

turtle.left(120)
turtle.forward(side_length*2)

turtle.right(120)
turtle.forward(side_length)

turtle.right(120)
turtle.forward(side_length*2)



# Question 4 Answer:
import turtle

turtle.color("red")
turtle.pensize(1)

for i in range(50):
    turtle.forward(50)
    turtle.left(110)

turtle.penup()
turtle.setpos(72, -33)

turtle.pendown()
turtle.color("blue")
for i in range(80):
    turtle.forward(120)
    turtle.left(115)

```
