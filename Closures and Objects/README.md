As you know Javascript has two different ways to treat the data it receives as arguments of a function:

* Primitives are passed by copy
* Complex Objects are passed by reference.

This mini-challenge is related with this topic.

	var oPerson = { name: 'john'};						// Define an object

	(function(oTeacher) {								// Create a closure to use the object in other function code.
	   window.getTeacher= function() {
		  console.log(oTeacher);
	   };
	}(oPerson));

	window.getTeacher();								// Get the teacher.

	oPerson.surname = 'doe';							// Augment the object.

	window.getTeacher();								// Get the teacher again.

	oPerson = { name: 'mary', surname: 'sullivan' };	// Redefine an object

	window.getTeacher();								// Get the teacher again.

The first execution of window.getTeacher returns:

	Object {name: "john"}

The second execution of window.getTeacher returns:

	Object {name: "john", surname: "doe"}

The third execution of window.getTeacher returns:

	Object {name: "john", surname: "doe"}

Can you explain what's the reason of this behaviour?

Can you see any problem about this behaviour?

How you could solve it?