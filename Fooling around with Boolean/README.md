Look at the following "implementation" of a xor method on the prototype of the Boolean type.

	Boolean.prototype.xor = function (sValue) {return !!this !== !!sValue};

Now, why does the following statement resolve in an unexpected manner?

	false.xor (false) // => true

What can you do to fix it and what is the term that describes this behaviour?

## Bonus!!

If all of the following statements are true

	!!{} == true
	[] == false

Why does calling ...

	hasTruthyStuff([{},[] 0])

... on the following function return false?

	var hasTruthyStuff = function (aSymbols) {
		var nResult = 0,
			i = 0
			nLen = aSymbols.length;

		for (; i < nLen; i++) {
			nResult |= aSymbols[i];
		}
		return !!nResult;
	};
