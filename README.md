Optimizations for index.html
------------------------------------------------------------------------
 - saved images in the img directory.
 - set the javascript to async
 - changed css to inline
 - updated metatag http://www.metatags.info/meta_name_expires
 - included cache control from example at http://www.mobify.com/blog/beginners-guide-to-http-cache-headers/
 - scored 92 / 100



 Optimizations for pizza.html
------------------------------------------------------------------------
- changes to main.js

- in the updatePositions function
	moved phase math var and for loop to after performance.mark timing activities.
	moved phase var declaration back inside of loop
	added + (i % 5) back to the phase variables math, which brings back the randomly shifting pizzas
	used getElementsByClassName instead of querySelectorAll

- in changePizzaSizes function
	Added Comments
	used getElementsByClassName instead of querySelectorAll
	moved var declarations to outside of loop

 - Load times
 	Time to generate pizzas on load: 35.23799998220056ms main.js:483 
	Average time to generate last 10 frames: 0.03349999897181988ms main.js:496 
	Average time to generate last 10 frames: 0.02829998265951872ms main.js:496
	Time to resize pizzas: 1.6790000954642892ms main.js:467	
