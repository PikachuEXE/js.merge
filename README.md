JavaScript/NodeJS Merge v1.1.0
==================================================

What is it?
--------------------------------------

JavaScript/NodeJS Merge is a tool to merge multiple objects into one object, with the possibility of create a new object cloned. His operation is very similar to the [jQuery.extend](http://api.jquery.com/jQuery.extend/) function but more flexible.

Example from NodeJS
--------------

	var merge = require('merge'), // npm install -g merge
		original, cloned;
	
	console.log(
		
		merge({ one: 'hello' }, { two: 'world' })

	); // {"one": "hello", "two": "world"}
	
	original = { x: { y: 1 } };

	cloned = merge(true, original);

	cloned.x.y++;

	console.log(original.x.y, cloned.x.y); // 1, 2

Example from JavaScript browser
--------------------------

	<script src="http://yeikos.googlecode.com/files/merge.js"></script>
	
	<script>
		
		var original, cloned;
		
		console.log(
			
			merge({ one: 'hello' }, { two: 'world' })
	
		); // {"one": "hello", "two": "world"}
		
		original = { x: { y: 1 } };
	
		cloned = merge(true, original);
	
		cloned.x.y++;
	
		console.log(original.x.y, cloned.x.y); // 1, 2

	</script>