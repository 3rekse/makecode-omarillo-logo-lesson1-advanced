### @explicitHints true

# Turtle Logo - Lesson #1 - Advanced

## Turtle Logo - Lesson #1, with variables and sprites @unplugged
**Welcome to coding with Turtle Logo.**

In this lesson you will create your first Turtle Logo program, using variables and sprites. You will get a **Turtle Object** showing up in your game console and have it say, "Hello, World!".
![Hello, World!](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson1-advanced/raw/main/assets/hello_world_screenshot.png)

## Step 0
** Technical Stuff**

Before you begin coding, you need to ensure you understand what variables are in programming and how to use them. A variable is just a memory location that the program uses to hold information. To create a variable you use the "Variables" menu and select "Make a Variable".

## Step 00
** Technical Stuff**

Next the term "sprite" will also be used. A *sprite* is just a 2D image that will show up in our game console.

## Step 000
** Follow Along**

Create a variable called "myDuck".
```blocks
let myDuck = null
```

## Step 1
** Follow Along**

All our programs begin with an ⇢``on start``⇠ block. This block runs all the commands that are inside it as soon as the program begins. It has been provided for you below. If you accidentally delete the block, you can find it under the *"Loops"* menu.
```blocks
/**
 * This is the "on start" block
 */
```

## Step 2
** Follow Along**

Next you will need to create your **Turtle Object**. To do this you use the ⇢``set myTurtle to a Turtle Object with sprite □ of kind Player``⇠ block and place it inside the ⇢``on start``⇠ block. This creates the **Turtle Object**. This object is being held in the default variable "myTurtle". The variable we previously created was "myDuck", so we will change this variable to ours.
```blocks
let myDuck = turtle.fromSprite(sprites.create(img``, SpriteKind.Player))
```

## Step 2.1
** Follow Along**

By default the sprite that our Turtle Object contains is nothing. We can select the sprite box and then either draw one or select one from the gallery. Select the "duck" from the gallery.
```blocks
let myDuck = turtle.fromSprite(sprites.create(img`
    . . . . . . . . . . b 5 b . . . 
    . . . . . . . . . b 5 b . . . . 
    . . . . . . b b b b b b . . . . 
    . . . . . b b 5 5 5 5 5 b . . . 
    . . . . b b 5 d 1 f 5 5 d f . . 
    . . . . b 5 5 1 f f 5 d 4 c . . 
    . . . . b 5 5 d f b d d 4 4 . . 
    . b b b d 5 5 5 5 5 4 4 4 4 4 b 
    b d d d b b d 5 5 4 4 4 4 4 b . 
    b b d 5 5 5 b 5 5 5 5 5 5 b . . 
    c d c 5 5 5 5 d 5 5 5 5 5 5 b . 
    c b d c d 5 5 b 5 5 5 5 5 5 b . 
    . c d d c c b d 5 5 5 5 5 d b . 
    . . c b d d d d d 5 5 5 b b . . 
    . . . c c c c c c c c b b . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player))
```

## Step 3
** Follow Along**

Now that we have a **Turtle Object**, you can ask it to say something. Drag out the ⇢``myTurtle says "Hello, World!" ⊕``⇠ block and place it inside the ⇢``on start``⇠ block but under the previous block. you will once again have to change the variable, to refer to the one you are using, "myDuck".
```blocks
let myDuck = turtle.fromSprite(sprites.create(img`
    . . . . . . . . . . b 5 b . . . 
    . . . . . . . . . b 5 b . . . . 
    . . . . . . b b b b b b . . . . 
    . . . . . b b 5 5 5 5 5 b . . . 
    . . . . b b 5 d 1 f 5 5 d f . . 
    . . . . b 5 5 1 f f 5 d 4 c . . 
    . . . . b 5 5 d f b d d 4 4 . . 
    . b b b d 5 5 5 5 5 4 4 4 4 4 b 
    b d d d b b d 5 5 4 4 4 4 4 b . 
    b b d 5 5 5 b 5 5 5 5 5 5 b . . 
    c d c 5 5 5 5 d 5 5 5 5 5 5 b . 
    c b d c d 5 5 b 5 5 5 5 5 5 b . 
    . c d d c c b d 5 5 5 5 5 d b . 
    . . c b d d d d d 5 5 5 b b . . 
    . . . c c c c c c c c b b . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player))
myDuck.say("Hello, World!")
```
## Step 4
**Success!**

Notice in the game console to the left, your **Turtle Object** said "Hello, World!" for 5 second and then the words vanish. If you want to run your program again, click the "🔁" button on the game console. You can also click the "⊕" and change the milliseconds to a larger number, to make it stay longer.
```blocks
let myDuck = turtle.fromSprite(sprites.create(img`
    . . . . . . . . . . b 5 b . . . 
    . . . . . . . . . b 5 b . . . . 
    . . . . . . b b b b b b . . . . 
    . . . . . b b 5 5 5 5 5 b . . . 
    . . . . b b 5 d 1 f 5 5 d f . . 
    . . . . b 5 5 1 f f 5 d 4 c . . 
    . . . . b 5 5 d f b d d 4 4 . . 
    . b b b d 5 5 5 5 5 4 4 4 4 4 b 
    b d d d b b d 5 5 4 4 4 4 4 b . 
    b b d 5 5 5 b 5 5 5 5 5 5 b . . 
    c d c 5 5 5 5 d 5 5 5 5 5 5 b . 
    c b d c d 5 5 b 5 5 5 5 5 5 b . 
    . c d d c c b d 5 5 5 5 5 d b . 
    . . c b d d d d d 5 5 5 b b . . 
    . . . c c c c c c c c b b . . . 
    . . . . . . . . . . . . . . . . 
    `, SpriteKind.Player))
myDuck.say("Hello, World!", 30000)
```

## Step 4
**Your Turn**

Get the **Turtle Object** to say your name!

## Step 5
**Done**

You have successfully completed your first lesson in Turtle Logo.
