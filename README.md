# FE-Interview-Questions

# Frontend Interview Questions

1. What is IIFE?
Immediately Invoked Function   
It creates a closure around the code and is a way to execute it immediately as soon as they are created.
	

2. What is ‘this’ keyword in JS and what does it bind to?

>It is a reference to an object which is being used outside a function, this refers to a global object, for example this.window
>ES6 doesn’t have this, they inherit from the parent, using arrow functions.

3. What is the different between absolute, relative, static positions in css?

Relative: is means relative to its normal position, top, bottom, left, right
Static: as the name suggests is always positioned according to the normal flow of the page
Absolute: is positioned relative to the nearest positioned ancestor

4. What are the three parts of an http request?


	1. Pre flight, client establishes the connection, usually this is TCP,  http server, default port is 80
	2. Client sends request to a web browser (GET/POST)
	3. After the request the server process it and returns a response, most important is the status code 200, 303, etc…

# WHITEBOARD QUESTIONS:

1. Add two values
	  function add(a,b){
		  return a + b; 	}

	  console.log(add(1,2))
	

2. Write a function that removes odd numbers from an array of numbers

	  function removeOddNumbers(array) {
  		  return array.filter(item => item % 2 === 0)
	  }

	  console.log(removeOddNumbers([1,2,3,4,5,6]))

3. Return an array of its values plus the value’s index
	
	  var array = [1,2,3,4,5,6]

	  console.log(array.map((w, index) => w + index))

4. Flatten a multidimensional array

	  function flatten(array) {
		  return array.reduce((flat, toFlatten) => {
			  return flat.concat(Array.isArray(toFlatten) ? flatten(toFlatten) : toFlatten)
		  }, [])
	  }

	  console.log(flatten([[1,-1,-3,-4], [2,3], [4]]))

	- Shuffle an array of integers 

	
