```
import turtle

t = turtle.Turtle()
t.speed(5)

# Функція для малювання щита
def draw_shield():
    t.penup()
    t.goto(-100, 100)
    t.pendown()

    t.begin_fill()
    t.fillcolor("blue")

    t.forward(200)
    t.right(90)
    t.forward(150)

    # Низ щита (закруглений)
    t.circle(-100, 180)

    t.forward(150)
    t.right(90)
    t.forward(200)

    t.end_fill()

# Функція для малювання хреста
def draw_cross():
    t.penup()
    t.goto(0, 50)
    t.pendown()

    t.color("yellow")
    t.pensize(10)

    # Вертикальна лінія
    t.setheading(-90)
    t.forward(120)

    # Горизонтальна лінія
    t.penup()
    t.goto(-50, 0)
    t.pendown()
    t.setheading(0)
    t.forward(100)

# Малюємо герб
draw_shield()
draw_cross()

turtle.done()

```
