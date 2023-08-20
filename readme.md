# Changes made to your code

## No. 1 - File structure changes.

- Anytime you are working with html you need an "index.html" file. That file tells the browser where the starting point of your website is.
- The main file for your CSS is called "styles.css" and should generally live in the same directory.

## No. 2 - Style Location change

I removed the styles from your html file because it makes your code easier to read.

## N0.3 - Code Changes

- Removed useless div "mainconverter". Applied the styles to "mainconvertera"
- Changed "mainconvertera" -> "converter-container" because it is more descriptive that way "container" tells another developer that it holds more content in it. It could also be named as "converter-card".
- Removed the "select" class on the selects and inputs and instead selected all "select" and "input" **elements** with the css selector. Naming a class after an element is unnecessary because you can select an element directly in CSS.
- Changed "UnitsIn" and "UnitsOut" to "unit-in" and "unit-out" as this is the naming convention for classes, id's and so on. Same for "tempi" -> "temp-in"
- Removed the id's on the temp-in select because it has name field. You do not need both. Just use "getElementByName"
- Moved all the variables containing the selects and inputs outside of the function so that they have global scope. That way you do not need to create a variable for them everytime you need them.
- The rest of the changes are made as comments in the javascript.
