Optimizations for pizza.html
------------------------------------------------------------------------
- changes to main.js

- in the updatePositions function
	moved   var phase = Math.sin((document.body.scrollTop / 1250) + (i % 5));
	to outside of its loop and changed it to...
	var phase = Math.sin(document.body.scrollTop / 1250);

- in changePizzaSizes function
	replaced var dx = determineDx(document.querySelectorAll(".randomPizzaContainer")[i], size);
    with var dx = determineDx(randomPizzaContainer[i], size);