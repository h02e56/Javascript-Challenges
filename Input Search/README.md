Reviewing the code of your colleague you have found this snippet of code:

	$( document ).ready( function() {
	  $( '#inputSearch' ).keypress( function() {
		  $.ajax( {
		  	url: 'http://xxxxxxx.domain.com/xxxx',
		  	data: this.value,
		  	success: function ( data )
		  	{
		  		var results = data.results;
		  		$( '#list' ).empty();
		  		$.each( data, function ( item ) {
		  			$( '#list' ).append( '<li>' + item + '</li>' );
		  		} );

		  	},
		  	error: function ( xhr, status, error ) {
		  		console.log( 'Something goes wrong!', status, error.message );
		  	}
		  } );
	  } );
	} );


What is/are the problem/s in this code?

How can you solve it/them?