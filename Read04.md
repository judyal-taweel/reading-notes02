# java scirept:
allows you to make web pages more interactive by accessing and modifying the content and markup 
used in a web page while it is being viewed in the browser.

can by java scirept Select any elements that have a
class attribute with a value of note.

### EXAMPLES OF JAVASCRIPT IN THE BROWSER 

- Access: the content of the page
- Modify: the content of the page
- Program: rules or instructions the browser can follow
- React: to events triggered by the user or browser 

##### like:
- A button is pressed
- A link is clicked (or tapped) on
- A cursor hovers over an element
- Information is added to a form
- An interval of time has passed
- A web page has finished loading

#### Start with what you want to achieve, and break
that down into smaller steps: 

1. DEFINE THE GOAL
2. DESIGN THE SCRIPT
3. CODE EACH STEP

Often scripts will need to perform different tasks in different situations.
You can use flowcharts to work out how the tasks fit together.
The flowcharts show the paths between each step. 

# FLOWCHART KEY

Generic step | Event
------------ | -----
Input or output | Decision 

### EXPRESSIONS

1. EXPRESSIONS THAT JUST ASSIGN A VALUE TO A VARIABLE
   `var color = 'beige';` 


1. EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE
   `var area = 3 * 2;`

### OPERATORS 

Expressions rely on things called operators; they allow programmers to
create a single value from one or more values. 

1. ASSIGNMENT OPERATORS
   `color = 'beige';`

1. ARITHMETIC OPERATORS
   `area = 3 * 2;`

1. STRING OPERATORS
   `greeting= 'Hi 1 + 'Mol ly';`

1. COMPARISON OPERATORS
   `buy = 3 > 5;`

1. LOGICAL OPERATORS
   `buy= (5 > 3) && (2 < 4);`

 #### Example on using arithmatic operation in java scirept:

`var subtotal (13 + 1) * 5; II Subtotal is 70`

`var shipping 0.5 * (13 + 1) ; II Shipping is 7`

`var total subtotal + shipping ; II Total is 77`

`var el Sub document .getElementByid(' subtotal ') ;`

`elSub .textContent =subtotal ;`

`var elShip = document .getElement Byid('shi ppi ng ') ;`

`elShip.textContent =shipping;`

`var elTotal = document .getElementByid('total ');`

`elTotal .textContent =total;`


#### Example on using mixing numbers and strings together in java scirept:

`var number = 12;`

`var street= 'Ivy Road';`

`var add = number + street;`
