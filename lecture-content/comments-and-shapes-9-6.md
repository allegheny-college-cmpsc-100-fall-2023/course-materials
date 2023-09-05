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

VPython offers a variety of built-in shapes that you can render in your 3D canvas. These shapes are instantiated as a dictionary datatype, which is something that we'll learn in more detail later in the semester. For now, you just need to know that you can store a shape inside a variable by calling its name followed by a set of empty parens <b>()</b>. You can then change certain attributies of that shape by referencing the variable and putting a period <b>.</b> between the variable name and the attribute:

```
big_ball = sphere() #stores a sphere inside of the variable named big_ball
big_ball.radius = 10 #sets big_ball's radius

small_ball = sphere() #stores another sphere inside of the variable named 
small_ball.radius = 2 #sets small_ball's radius
small_ball.pos = vector(10, 10, 10) #sets small_ball's position

```

Some of these attributes have attributes of their own. For example, if we added the following line to the code above...

```
small_ball.pos.x = 20 #changes small_ball's position along the x axis

```

...the small ball would move right by 10 units. (Note that generally Python renders in order from top to bottom, so whichever position is last in the code is the position we will see on the screen.)

Variables are useful not just for storing these shapes so that we can maniupate them. They are also useful for if we want to use the same value a bunch of times, especially if that value may change. Like let's say you knew you wanted all your shapes to sit neatly a row, but you wanted flexibility on where that row was positioned. You could write code something like this. 

```
row_y = 5 #establishes y coordiante for row of shapes
row_z = 0 #establishes z coordinate for row of shapes

brick = box() #draws a box and stores it in variable "brick"
brick.pos = vector(-2, row_y, row_z) #sets the position of brick
brick.size = vector(2, 2, 2) #sets the length, height, and width of brick

ball = sphere() #draws a sphere and stores it in variable "ball"
ball.pos = vector(1, row_y, row_z) #sets the position of ball
ball.radius = 1 #sets the radius of ball

pyr = pyramid() #draws a pyramid and stores in variable "pyr"
pyr.pos = vector(3, row_y, row_z) #sets the position of pyr
pyr.size = vector(3, 3, 2) #sets the length, height, and width of pyr


```

Note we haven't written a variable for x, and that is because different shapes will have different x coordinates. If they all had all three coordinates the same, they would sit right on top of each other! (Try changing the code to see for yourself.)

Helpful Resources: 
-[VPython Sphere](https://www.glowscript.org/docs/VPythonDocs/sphere.html)
-[VPython Box](https://www.glowscript.org/docs/VPythonDocs/box.html)
-[VPython Pyramid](https://www.glowscript.org/docs/VPythonDocs/pyramid.html)
