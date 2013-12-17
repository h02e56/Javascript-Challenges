Today we are going to see how to ‘solve’ a problem using one of the new features in (JavaScript 1.8.5) this feature is Object.freeze.
This is the challenge:

	var oDog = {

		sound: ‘Bark!’

	};

	Object.freeze(oDog);

	/*Put you code here*/

	oDog.talk();      // This method should launch an alert with the text ‘Bark’.

Assume:

* There is no more code than this lines.
* You can use anything of ECMASCRIPT 5 but not DOM or BOM, just Javascript.
* There are more than one answer but only the most simple will win.