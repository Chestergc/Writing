# On the topic of Behaviors
## or how to apply games development workflow into software development

To develop a computer program most programmers think about the system and the functions that need to be defined for the program to work as intended.

Most people think about objects and how they interact with one another, making simple chains of objects interacting to develop the actual programming function needed to describe the functionality a certain piece of the code will implement.

Which is what brings back the topic of how to program software, object oriented programming is accepted by programmers and engineers alike, for the most part it surely is the simplest way to implement most software and without a shadow of a doubt is the quickest way to implement any software.

In the past couple of years researchers and engineers have been hit by a sudden realization, it may not be the best way to do this.

For the most part object oriented programming is actually the best way to think about any program, functional programming is not as easy to think about as objects arranged inside a program.

Let a simple program be defined as such:
```py
class Animal:
  def__init__(self, color, legs):
    self.color = color
    self.legs = legs
```
This program would describe an object in the class Animal, which could then be used to instantiate participants of the class with the functionality defined inside of the actual class, it could be overwritten and redefined in the inherited object, but that would have to be done in a case by case basis, which could be quite cumbersome and time consuming, although infinitely faster than functional programs, where you would need to rewrite that portion of the code every time you needed a function that is almost like that but not quite. Such as:
```py
def animal():
  animalcolor = color
  animallegs = legs
```
It is still, quite (*ahem*) functional, although you would have to rewrite the code quite a lot, that would inevitably become a complicated and laborious task, with the programmer needing to keep in mind several rewrites of the code.

In the past few weeks I've been struck with a conundrum, which text editor should I be using? I've tested all the usual suspects, sublime text, atom, light table and all of them had their ups and downs, but not one of them had everything I would need from a text editor for my personal use, I am currently taking a course to become a mechatronics technician and for that purpose I would need a few simple things in my text editor; a simple way to edit hexadecimal or binary files, integration with git, compilers of many different varieties, being able to open schematics in pdf inside of the editor, being able to make spreadsheets would be good, but not required. And for that exact purpose I haven't found, any text editor that did everything, so I started digging into the core files of them, thinking about writing my own plugins for the things I needed to do, which led me to another way to think about programs, the way light table does it, BOT architecture.

BOT stands for Behavior, Object, Tag, and that programming architecture is all about defining actions before objects, and then assigning tags to the objects, making them accessible from higher up in the stack.

In a program you can see yourself using this type of architecture to describe things a function could do without inheriting from a class. The main point is discovery time, the amount of discovery that can be done this way makes such that you are able to implement new features faster and test around the program simply, because you can just test the behaviors and see what they do to understand what the object can and can't do. That is the way I thought about programming games, if you get stuck on what should the character be able to do you can borrow a behavior from an enemy or a bit of scenery and see what happens, maybe that would turn out to be a fun and implementable skill for the main character, making a new portion of the game based around that could turn out to be fun.

The way to think about this type of architecture is to think about behaviors as actions and tags as ways to access them from the interface, such as:
```py
def color(str x):
  color=x
  return color

def legs(str x):
  legs=x
  return legs

def animal():
  color()
  legs()
```
And then when you have another object that would have the same behaviors you could use the same ones you already defined:
```py
def dog():
  color():
  legs():
```
And then you can assign tags to be able to access them from other functions.
```py
def dog(x):
  if x==1:
    return color(dog)
  elif x==2:
    return legs(dog)
  else:
    return 0
```
This way of thinking about programs makes it so that features are easily implemented and new ideas are quickly discovered, making programs easier to implement and ideas easier to discover.

Guilherme Chimello
