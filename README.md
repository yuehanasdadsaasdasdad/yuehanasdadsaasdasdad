import turtle
import time

# Set up the screen
screen = turtle.Screen()
screen.bgcolor("white")

# Create a turtle for drawing the text
text_turtle = turtle.Turtle()
text_turtle.speed(1)  # Set the drawing speed
text_turtle.pensize(3)  # Set pen size

# Function to write "I LOVE YOU" from top to bottom with a duration
def write_love_message():
    text_turtle.penup()
    text_turtle.goto(0, -10)  # Start at the top of the screen
    text_turtle.pendown()

    # Set the font style and write each word with a duration
    text_turtle.color("red")
    text_turtle.write("I", align="center", font=("Arial", 24, "bold"))  # Small font size
    time.sleep(1)  # Pause for 1 second

    text_turtle.color("purple")
    text_turtle.goto(0, -60)  # Move down to the next position
    text_turtle.write("LOVE", align="center", font=("Arial", 24, "bold"))  # Small font size
    time.sleep(1)  # Pause for 1 second

    text_turtle.color("blue")
    text_turtle.goto(0, -100)  # Move down to the next position
    text_turtle.write("YOU", align="center", font=("Arial", 24, "bold"))  # Small font size
    time.sleep(1)  # Pause for 1 second

    text_turtle.color("purple")
    text_turtle.goto(0, -140)  # Move down to the next position
    text_turtle.write("MWA", align="center", font=("Arial", 24, "bold"))  # Small font size
    time.sleep(1)  # Pause for 1 second

# Draw the message
write_love_message()

# Hide the turtle after drawing
text_turtle.hideturtle()

# Keep the window open until clicked
screen.exitonclick()
