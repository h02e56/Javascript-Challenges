This code should exit the first time indexInnerLoop has a value of 10 and indexOuterLoop should log 0.

    var indexOuterLoop, iterationsOuterLoop = 1000, indexInnerLoop, iterationsInnerLoop = 100;

    for (indexOuterLoop = 0; indexOuterLoop < 1000; indexOuterLoop++)
    {
         for (indexInnerLoop = 0; indexInnerLoop < iterationsInnerLoop; indexInnerLoop++)
         {
            if (indexInnerLoop === 10)
            {
                 break;
            }
         }
    }

    console.log( indexOuterLoop );  // Should log 0.

Is possible to accomplish the requirements?

What are the modifications can you do to perform the requirements?

Why?