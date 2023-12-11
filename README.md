### @explicitHints true

# Turtle Logo - Lesson #1 - Advanced

## Turtle Logo - Lesson #1, Programmiamo utilizzando variabili e sprite @unplugged
**Welcome to coding with Omarillo Logo.**

In questa lezione creerai il tuo primo programma per Omarillo, utilizzando variabili e sprite. Verrà visualizzato un **Oggetto Tartaruga** nella tua console di gioco e dirà "Ciao, mondo!", come  **Turtle Object**  dice :
![Hello, World!](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson1-advanced/raw/main/assets/hello_world_screenshot.png)

## Step 0
** Technical Stuff**

Prima di iniziare a scrivere codice, devi assicurarti di comprendere quali variabili sono presenti nella programmazione e come utilizzarle. Una variabile è semplicemente una posizione di memoria utilizzata dal programma per conservare le informazioni. Per creare una variabile utilizzare il menu "Variables/Variabili" e selezionare "Make a Variable/Crea una variabile".

## Step 00
** Technical Stuff**

Successivamente verrà utilizzato anche il termine "sprite". Uno *sprite* è semplicemente un'immagine 2D che verrà visualizzata nella nostra console di gioco.

## Step 000
** Follow Along**

Crea una variabile chiamata "myDuck".
```blocks
let myDuck = null
```

## Step 1
** Follow Along**

Tutti i nostri programmi iniziano con un ⇢``on start``⇠ block. 
Questo blocco esegue tutti i comandi che si trovano al suo interno non appena inizia il programma. Ti è stato fornito di seguito. Se elimini accidentalmente il blocco, puoi trovarlo nel menu *"Loops"* .
```blocks
/**
 * This is the "on start" block
 */
```

## Step 2
** Follow Along**

Successivamente dovrai creare il tuo **Oggetto Omarillo**. Per fare ciò utilizza ⇢``set myTurtle to a Turtle Object with sprite □ of kind Player``⇠ block e posizionarlo all'interno del ⇢``on start``⇠ block. 
Questo crea l'**Omarillo Object**. Questo oggetto viene mantenuto nella variabile predefinita "myTurtle". La variabile che abbiamo creato in precedenza era "myDuck", 
quindi cambieremo questa variabile nella nostra.
```blocks
let myDuck = omarillo.fromSprite(sprites.create(img``, SpriteKind.Player))
```

## Step 2.1
** Follow Along**

Per impostazione predefinita, lo sprite contenuto nel nostro oggetto Tartaruga non è nulla. Possiamo selezionare la casella dello sprite e poi disegnarne una o selezionarne una dalla galleria. Seleziona la "duck" dalla galleria.

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
