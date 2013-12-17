Having this code:

	function Order()
	{
			 this.aOrderLines = [];
			 this.nOrderTotal = 0;
	}
	Order.prototype.getOrderLines = function()
	{
			 return this.aOrderLines;
	};
	Order.prototype.addOrderLine = function(oOrderLine)
	{
			 this.nOrderTotal += oOrderLine.nTotal;
			 this.aOrderLines.push(oOrderLine);
	};
	Order.prototype.removeOrderLine = function(oOrderLineItem)
	{
			 var nOrderTotal;
			 oOrderLine = this.aOrderLines.map(function(oOrder)
			 {
					  return oOrder === oOrderLineItem;
			 })[0];

			 if(typeof oOrderLine === 'undefined' || oOrderLine === null)
			 {
					  return;
			 }
			 this.nOrderTotal -= oOrderLine.nTotal;
			 this.aOrderLines.splice(this.nOrderTotal, 1);
	};

The problem in this code is that anyone could access aOrderLines and add or modify values without increasing or decreasing nOrderTotal.

Keep in mind that you have to implement a method to get aOrderLines to loop over its items but avoiding to modify the values.

How you could solve this problem?

