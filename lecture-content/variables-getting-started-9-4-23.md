# September 4, 2023

### Code along with me!

<img src = 'https://github.com/allegheny-college-cmpsc-100-fall-2023/course-materials/assets/8368413/675714d9-2e56-46b5-a999-20960b04c065' width = '400px' />


### <em> or </em>
### Watch and take notes!

<img src = 'https://github.com/allegheny-college-cmpsc-100-fall-2023/course-materials/assets/8368413/89180da5-1cd0-408e-9af0-fdb47700825f' width = '400px' />

### <em>however you learn best!</em>


## Variables, a quick introduction

Variables are containers: they can hold a variety of different values. You could imagine a variable as a tea bag, and its value as the kind of tea the bag holds. While the procedure might be the same for different kinds of tea, the flavor will vary depending on the contents of the bag. Wherever a variable appears in code, it deploys the value it contains, much as a teabag releases its flavors when placed in hot water. Variables allow programs to respond to varying stimuli differently, and this is powerful.

In Python, variables are assigned using the following syntax:

```
variable_name = variable_value
```
Even if you’ve never coded before, you might be familiar with the concept of a variable from taking algebra in school. In the example below, variables hold values, just like in algebra; however, the variables below hold text rather than numbers.

so... 
  
```
pet_type = "cat"
pet_name = "Fifi"
print( "My "  + pet_type + "'s name is " + pet_name)
#outputs "My cat's name is Fifi" 

pet_type = "dog"
pet_name = "Sparky"
print( "My "  + pet_type + "'s name is " + pet_name)
#outputs "My dog's name is Sparky"
  
```
Notice the above variable values are all in quotes. That's because they are text, known in computer science as the <b>string</b> datatype. The quotes tell Python to treat the values as text. Numerical values are assigned without quotes, and Python knows to treat them accordingly: 

```
a = 2
b = 3
print(a + b)
#outputs 5

a = "2"
b = "3"
print(a + b)
#outputs 23
```
