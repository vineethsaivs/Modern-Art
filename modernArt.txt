from turtle import *
from random import *

colormode(255)
def randomcolour():
    red = randint(0, 255)
    green = randint(0, 255)
    blue = randint(0, 255)
    color(red, green, blue )

def randomplace():
    penup()
    x = randint(-100,100)
    y = randint(-100,100)
    goto(x,y)
    pendown()

def randomheading():
    heading = randint(0, 360)
    setheading(heading)

shape("turtle")
speed(0)
for i in range(4):
    randomcolour()
    randomplace()
    randomheading()
    stamp()

def drawrectangle():
    randomcolour()
    randomplace()
    hideturtle()
    length = randint(10, 100)
    height = randint(10, 100)
    begin_fill()
    forward(length)
    right(90)
    forward(height)
    right(90)
    forward(length)
    right(90)
    forward(height)
    right(90)
    end_fill()

clear()
setheading(0)

for i in range(20):
    drawrectangle()
from turtle import *
from random import *

def randomcolour():
    red = randint(0, 255)
    green = randint(0, 255)
    blue = randint(0, 255)
    color(red, green, blue )

def randomplace():
    penup()
    x = randint(-100,100)
    y = randint(-100,100)
    goto(x,y)
    pendown()

def randomheading():
    heading = randint(0, 360)
    setheading(heading)

shape("turtle")
speed(0)
for i in range(4):
    randomcolour()
    randomplace()
    randomheading()
    stamp()

def drawrectangle():
    randomcolour()
    randomplace()
    hideturtle()
    length = randint(10, 100)
    height = randint(10, 100)
    begin_fill()
    forward(length)
    right(90)
    forward(height)
    right(90)
    forward(length)
    right(90)
    forward(height)
    right(90)
    end_fill()
    
def drawcircle():
  radius = randint(5, 100)
  randomcolour()
  randomplace()
  dot(radius)
  
def drawstar():
  randomcolour()
  randomplace()
  randomheading()
  begin_fill()
  size = randint(20, 100)
  #draw the star shape
  for side in range(5):
    left(144)
    forward(size)

  end_fill()

clear()
setheading(0)

for i in range(20):
    drawrectangle()
    
clear()

for i in range(20):
  drawcircle()
  
clear()

for i in range(20):
  drawstar()
