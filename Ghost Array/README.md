Take a look at this code:

    var arr = [];

    arr[999] = 'john';

    console.log( arr.length );              // Question 1
    console.log( arr[999] );                // Question 1.1

    var arr_1 = [];
    arr_1[4294967295] = 'james';

    console.log( arr_1.length );            // Question 2
    console.log( arr_1[4294967295] );       // Question 2.1

    var arr_2 = [];
    arr_2[Number.MIN_VALUE] =  'mary';

    console.log( arr_2.length );            // Question 3
    console.log( arr_2[Number.MIN_VALUE] ); // Question 3.1

What is the result of...

* Question 1 - Why?
* Question 1.1 - Why?


* Question 2 - Why?
* Question 2.1 - Why?


* Question 3 - Why?
* Question 3.1 - Why?
