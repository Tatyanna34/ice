# iceimport turtle

# Setup the turtle
screen = turtle.Screen()
screen.bgcolor("light blue")

snowflake = turtle.Turtle()
snowflake.color("white")
snowflake.speed(10)

# Function to draw one arm of the snowflake
def draw_arm():
    for _ in range(3):
        snowflake.forward(100)
        snowflake.backward(100)
        snowflake.right(45)
    snowflake.left(90)
    snowflake.backward(100)
    snowflake.left(45)

# Draw the snowflake by repeating the arm drawing 8 times
for _ in range(8):
    draw_arm()
    snowflake.left(45)

# Hide the turtle and display the window
snowflake.hideturtle()
turtle.done()
