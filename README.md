### @explicitHints true

# Turtle Logo - Lesson #1

## Turtle Logo - Lesson #1, with Sprites @unplugged
**Welcome to coding with Turtle Logo.**

In this lesson you will create your first Turtle Logo program, using variables and sprites. You will get a **Turtle Object** showing up in your game console and have it say, "Hello, World!".
![Hello, World!](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson1-advanced/raw/main/assets/hello_world_screenshot.png)

## Step 1
Code your solution below.

```ghost
let someVariableName = turtle.fromSprite(sprites.create(img`
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player))
someVariableName.say("Hello, World!")
```