# JavaScript

Windows . = emojis!

backticks allows gaps to fill in. 

boolean in objects interpolation.
    ${breakfast.coffee.decaf ? 'real': 'decaf'}
    use ${}.join(", ") to get spaces between array methods

7/19

'let' can be changed, const cannot be changed

FOR LOOP/FOR EACH
for each, is an array method

=> lambda

catNames.forEach(cat => console.log('forEach', cat))
    cat equals single element or catNames[i]

FILTER

let youngCats = cats.filter(cat => cat.age < 10)
console.log('young Cats', youngCats);
will produce separate array

FIND

let foundCat = null
for loop
    let cat
    if(cats.name == "sammie)...

If wants to find all items compared, use filter

function drawVillain()
empty string
for each loop puts name into template, use backtick and interpolation to print names
get element
log
innertext= printed objects to webpage
change to HTML to print to page

put quotes around curly brackets around curly braces to inhibit parsing into strings

when using v[property] to signify v.hair

7/20
// Adding items to list
// nav/background color
// rows/columns with items and ticket
// make empty array/add objects
// hardcode cards in html 'item name/price
// css styling/
//drawMenu() function - want to draw many items
    //create template
    //for each item, want to add to template/paste in hardcoded html
    //Add interpolation
    //drawMenu in console log to check
    getElembyID
    InnerHTML in JS

 Common Error-
 Cannot set a null as innerHTML
 If ...Element can't be found, will become null   

make cards clickable
quotes/interpolation on onclick
function order
    find items in array that match name that clicked
    (console log)

create empty array 'orders' and push foundCoffee Item

print to screen
    drawOrder()
    drawing many things so need template

    make html for order summary
    
    drawOrder after order function
    grab element and innerHTML

want running total
clear button

function drawTotal
    toFixed(2) includes 2 digits past the decimal

shift tab for decreasing indent

7/21

zookeeper
control shift z for color changes

background and links/html/js
headers/main container fluid
rows, cols, paddings, margins

create object/dictionary

key/value pairs

objects = animals.koko

drawfuction for array animals
    use forEach

objects use for-in loop
    let animal = animals[key] Use for dictionaries, key:value pairs.
        gets the single key:value pair in the dictionary

use animal.hunger for values from a specific key
use 'key' for html interpolation, only want the string
    if use key in animal.key, will only print the values


use id on the parent html

INTERVALS
write function that wants to happen

if statements for hunger

setInterval takes in 'handler'
    setInterval
    don't call 'hunger' just give instructions to run later (every so many seconds)

    onclick feed() and 
    
    can use to automatically find key in object

switch statement
 in the case of 'happy: += 10 cash...
 break
 default: 