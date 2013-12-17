What's happening when I execute this code?

	['1','10','100','1000','10000', '100000', '1000000'].map(parseInt)

To get this result:

	[1, NaN, 4, 27, 256, 3125, 46656]

How you could fix it? To get:

	[1,10,100,1000,10000, 100000, 1000000]
