# Computational Expression | September 6

## Code Comments

You might have noticed code comments in some of the class demonstrations. In Python, code comments are formatted either with a # at the beginning of the line for a single-line comment or end-of-line comment, or with three apostrophes at the start and the finish, for a multi-line comment. 

```
# a single line comment
# you can also put a comment at thh end of a line
pet = "cat" # assigns the value "cat" to the variable pet

'''
a
multi
line
comment
'''
```

When a line of text is "commented out," the code compiler skips it. Comments are not treated as code, and so you can put whatever you want inside them without messing up your project. 

Code comments are used to give plain-language information one what's going on, to help our future selves and collaborators understand our programs. This process of explaining what code is doing using code comments is called <b>documentation</b>, and it's a critical part of good programming.

Code comments can also be used to temporarily silence a line of code that you're not ready to delete. 

Helpful Resource: [Python Comments, W3Schools](https://www.w3schools.com/python/python_syntax.asp)

## Shapes in VPython

VPython offers a variety of built-in shapes that you can render in your 3D canvas. These shapes are instantiated as a dictionary datatype, which is something that we'll learn in more detail later in the semester. For now, you just need to know that you can store a shape inside a variable, then change certain properties of that shape by referenving the variable and then putting a <b> between the variable name and the property:

```
big_ball = sphere() #stores a sphere inside of the variable named big_ball
big_ball.radius = 10 #sets big_ball's radius

small_ball = sphere() #stores another sphere inside of the variable named 
small_ball.radius = 2 #sets small_ball's radius
small_ball.pos = vector(10, 10, 10) #sets small_ball's position


```

![ball example](image.png)

