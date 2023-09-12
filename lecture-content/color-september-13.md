# Working with Color

> Color is the most relative medium in art.
>> Josef Albers

- [Interaction of Color](https://github.com/allegheny-college-cmpsc-100-fall-2023/course-materials/assets/8368413/10cfbc6e-0c9c-4eef-a800-6480bff86bde)
- [Interaction of color | Plate IV-I](https://codepen.io/noraspice/full/aOggPw)
- [different reds](https://github.com/allegheny-college-cmpsc-100-fall-2023/course-materials/assets/8368413/e11c7818-268d-4bfb-b9f1-3e5e4824b90e)

## Variables and Perception

A variable is a symbol/placeholder for a value that may change.

Computer variables and natural language might not be as different as you’d think.

Different words and symbols can have different meanings for different people. They may even change over time for an individual. In the same way, the value inside a variable can change.

> What counts is not the what but the how
>> Josef Albers

## Color Tools

- [Adobe Color](https://color.adobe.com/)
- [Munsell Color System](https://pteromys.melonisland.net/munsell/)
- To convert RGB 256 colors to VPython vector colors
```
#colors encoded in 256 color RBG format
#(a format very commonly found onlin3)
r256 = 	0
g256 = 163
b256 = 108

#convert from 256 color scheme to 0-1
r1 = r256/255
g1 = g256/255
b1 = b256/255

t = pyramid() #draw pyramid
#color pyramid using converted colors
t.color = vector(r1, g1, b1) 

```
This example colors a pyramid a jade hue. [See the example on trinket.](https://trinket.io/library/trinkets/44eaa525a0) 
