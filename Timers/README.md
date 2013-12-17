When I execute this code:

	var check = false;
	var timeStart = new Date().getTime();

	setTimeout( function () {
		check = true;
	}, 1000 );

	while( !check ){
	}

	console.log( 'Loop has finished', 'Elapsed time:' + (new Date().getTime() - timeStart) );

When I will see the log in the console?

What will be the approximated value of the elapsed time?

Why?