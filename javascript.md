# FUNCTION

Functions let you group a series of statements together to perform a
specific task. If different parts of a script repeat the same task, you can
reuse the function (rather than repeating the same set of statements).

#### in HTML:

`<!DOCTYPE html>`

`<html>`

`<head>`

`<title>Basic Function</title>`

`<link rel ="stylesheet" href="css/ c03.css" />`

`</head>`

`<body>`

`<hl>TravelWorthy</ hl>`

`<div id="message">We lcome to our site! </ div>`

`<script src="js/ basic-function .js"></script>`

`</ body>`

`</ html>`

#### IN JAVASCRIPT:

`var msg = 'Sign up to receive our newsletter for 10% off!';`

`function updateMessage() {`

`var el = document.getElementByld('message'};`

`el .textContent = msg;`

`}`

![result](imgs/result.PNG)

### How to write the function:

function keyword `function` then function name `hello` then `{}` then write what you need into block

### Calling function:

function name `hello();`

### Declaring functions thet need information:

`function getArea(width, height){`
`return width*height;`
`}`

that need parameters are user like variables within the function.

### Calling functions that need information:

- arguments as values

`getArea(3,5);`

- argument as variables

`width = 3;`

`height = 5;`

`getArea(width,height);`

And can we calculate the arguments in functions .


