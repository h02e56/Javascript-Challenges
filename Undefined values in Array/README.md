See the next snippet of code:

	var aArr = [];
	aArr.length = 10;

	console.log(aArr);							// Shows [undefined, undefined, undefined, undefined, undefined, undefined, undefined, undefined, undefined, undefined] in the console.

	console.log( JSON.stringify( aArr[0] ) );	// Shows undefined in the console.


	console.log( JSON.stringify( aArr ) );		// Question 1

	console.log( aArr.toString() );				// Question 2

What will show the console in Question 1 ?  Why?

What will show the console in Question 2 ?  Why?