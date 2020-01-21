<!-- .slide: data-background="./Images/header.svg" data-background-repeat="none" data-background-size="40% 40%" data-background-position="center 10%" class="header" -->
# FEW 1.2 - Lesson 5 - OOP and JS Part 2

<!-- Put a link to the slides so that students can find them -->

➡️ [**Slides**](/Syllabus-Template/Slides/Lesson1.html ':ignore')

<!-- > -->

# Overview

This class will be an OOP workshop to review the concepts from the previous class.

<!-- > -->

### Why work with Classes and inheritance?

This is a big topic which reaches deeply into important areas of computer science. Expect to see OOP and inheritance in the libraries you might work with, in interview questions, and on the job as a software engineer. 

<!-- > -->

## Learning Objectives

1. Create base/superclasses 
1. Use inheritance with super and extends
1. Create classes that inherit from a superclass

<!-- > -->

# Inheritance 

Inheritance is when you get something from your ancestors. 

- genes
- money
- property

In software this could be: 

- variables/properties
- methods/functions

Who do you inherit from? 

- Your parents
- Your grandparents

In software who do you inherit from?

- Your parent/superclass

## Inheritence with JS

Any class can inherit from another. You can also think of classes that inherit from another class as extensions of the other class. 

```js
class Sprite {
 constructor() {
 this.x = 0
 this.y = 0
 }
}

class Ball extends Sprite {
 constructor() {
 super()

 this.radius = 10
 }
}

const ball = new Ball() // { x: 0, y: 0, radius: 10 }
```

Calling super() in a subclass is like calling the constructor function in your superclass. 

** You must call super()!**

If a class takes parameters in its constructor it must pass these to super. 

```js
class Sprite {
 constructor(x, y) {
 this.x = 0
 this.y = 0
 }
}

class Ball extends Sprite {
 constructor(x, y, color, radius) {
 super(x, y) // Must pass parameters to super!

 this.color = color
 this.radius = radius
 }
}

const ball = new Ball(10, 20, 'red', 30) 
// { x: 10, y: 20, color:'red', radius: 30 }
```

You must pass parameters to super. Notice the constructor takes these parameters, calling super is like calling the constructor of the superclass. 

<!-- > -->

# Using Inheritance

Pair with some at the same stage/level and work on the stretch challenges together.

<!-- v -->

<!-- .slide: data-background="#087CB8" -->
## BREAK

Take a 10-minute break and think about things in the world that share properties. 

<!-- > -->

# Workshop Problem Solving



<!-- v -->

## Overview/TT II (optional) (20 min)

<!-- v -->

## In-Class Activity II (optional) (30 min)

<!-- > -->

## Wrap Up

- Continue working on your current tutorial
- Complete reading
- Complete challenges

<!-- > -->

## Additional Resources

1. Links to additional readings and videos

<!-- > -->

## Minute-by-Minute [OPTIONAL]

| **Elapsed** | **Time** | **Activity** |
| ----------- | --------- | ------------ |
| 0:05 | 0:05 | admin |
| 0:15 | 0:10 | [Overview](#overview) |
| 0:20 | 0:05 | [Learning Objectives](#learning-objectives) |
| 0:50 | 0:30 | [Inheritence](#inheritence) |
| 1:00 | 0:10 | [BREAK](#break) |
| 2:25 | 1:30 | [Workshop problem solving](#workshop-problem-solving) |
| 2:45 | 0:20 | [Wrap up](#wrap-up) |
