After executing the next snippet of code...

    var key,
        obj = {
            name: 'john',
            surname: 'doe'
        };

    // Fill the code

    for ( key in obj ) {
        if ( obj.hasOwnProperty( key ) ) {
           console.log( key + ' exist in obj' );
           console.log( key + ': ' + obj[key] );
           continue;
        }
        console.log( key + " doesn't exist in obj" );
    }

... the console shows the next messages:

    name doesn't exist in obj
    name: john
    surname doesn't exist in obj
    surname: doe

Fill the code section with the code, to get the previous result, without modify obj.

Why this happens?