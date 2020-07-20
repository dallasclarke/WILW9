# What I learned Week-9.

 **process.argv** - Command line arguement similar to what we have used before (ex.getInput) to get user inputs inside of node.

 Heres how it's used:

 const userInput = process.argv[2];

 ---

 ## CSV (Comma seperated values).

 - We used csv files to import a bunch of data into JavaScript so that we could do something it. To import a CSV file into the editor is super simple and is done by doing the following:

const fs = require('fs');
const file = fs.readFileSync('./file-name.csv', 'utf-8');



## Two-dimensional arrays

- Two-dimensional arrays are a collection of items which share a common name and they are organized as a matrix in the form of rows and columns. The two-dimensional array is an array of arrays, so we create an array of one-dimensional array objects. 

## setInterval

The setInterval() method, offered on the Window and Worker interfaces, repeatedly calls a function or executes a code snippet, with a fixed time delay between each call. It returns an interval ID which uniquely identifies the interval, so you can remove it later by calling clearInterval().
-MND web docs.

- Inside of the parameters of setInterval we used a function and a time in milliseconds like so...

setInterval(functionName, time);

-clearInterval(functionName) stops the interval loop.

## setTimeout

- Sets a timer which executes a function or specified piece of code once the timer expires.
- Use clearTimeOut() to cancel the time out.
- Inside the parameters of setTimeOut() do the following:

setTimeOut(functionName, delay);

**Things to be aware of with setTimeOut**

- Be aware that setTimeout() and setInterval() share the same pool of IDs, and that clearTimeout() and clearInterval() can technically be used interchangeably. Make sure to always match them together or else code can be a mess.



