### @explicitHints true

# Turtle Logo - Lesson #1 - Advanced

## Turtle Logo - Lesson #1, Programmiamo utilizzando variabili e sprite @unplugged
**Welcome to coding with Omarillo Logo.**

In questa lezione creerai il tuo primo programma per Omarillo, utilizzando variabili e sprite. Verrà visualizzato un **Oggetto Omarillo** nella tua console di gioco e dirà "Ciao, benvenuti all'Omar di Oleggio!", come  **Turtle Object**  dice "Hello, Word!" :
![Hello, World!](https://github.com/Mr-Coxall/makecode-arcade-turtle-logo-lesson1-advanced/raw/main/assets/hello_world_screenshot.png)

## Step 0
** Technical Stuff**

Prima di iniziare a scrivere codice, devi assicurarti di comprendere il concetto di **variabile**, le variabili sono presenti nella programmazione e dobbiamo capire come utilizzarle. Una variabile è semplicemente una posizione di memoria utilizzata dal programma per conservare le informazioni. Per creare una variabile utilizzare il menu "Variables/Variabili" e selezionare "Make a Variable/Crea una variabile".

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

Successivamente dovrai creare il tuo **Oggetto Omarillo**. Per fare ciò utilizza ⇢``set myOmarilo to a Omarillo with sprite □ of kind Player``⇠ block e posizionarlo all'interno del ⇢``on start``⇠ block. 
Questo crea l'**Omarillo Object**. Questo oggetto viene mantenuto nella variabile predefinita "myOmarillo". La variabile che abbiamo creato in precedenza era "myDuck", 
quindi cambieremo questa variabile nella nostra.
```blocks
let myDuck = omarillo.fromSprite(sprites.create(img``, SpriteKind.Player))
```

## Step 2.1
** Follow Along**

Per impostazione predefinita, lo sprite contenuto nel nostro oggetto Tartaruga non è nulla. Possiamo selezionare la casella dello sprite e poi disegnarne una o selezionarne una dalla galleria. Seleziona la "duck" dalla galleria.

```blocks
let myDuck = omarillo.fromSprite(sprites.create(img`
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

Ora che abbiamo un **Oggetto Omarillo**, puoi chiedergli di dire qualcosa. Trascina fuori il ⇢``myOmarillo says "Hello, World!" ⊕``⇠ block e posizionarlo all'interno del ⇢``on start``⇠ blockma sotto il blocco precedente. dovrai ancora una volta modificare la variabile, per fare riferimento a quella che stai utilizzando, "myDuck".
```blocks
let myDuck = omarillo.fromSprite(sprites.create(img`
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
myDuck.say("Ciao, ciao!")
```
## Step 4
**Success!**
Puoi anche fare clic su "⊕" e cambiare i millisecondi con un numero più grande, per far rimanere il messaffio più a lungo

.
```blocks
let myDuck = omarillo.fromSprite(sprites.create(img`
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
myDuck.say("Ciao, ciao!", 30000)
```

## Step 4
**Tocca a te**

Ottieni l'**Oggetto Omerillo** che pronuncia il tuo nome!

## Step 5
**Done**

You have successfully completed your first advanced lesson in Omarillo Logo.
