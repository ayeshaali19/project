###### BUILT-IN ITERATION METHODS
## Other Built-In Methods

##### Go back to [**Simpler Is Better**](../ayesha/exercise4.md)  

Now, we know that not all for loops used just to print things to the console. For Loops can be used to manipulate arrays in many different ways, such as changing the items in an array or making decisions based on what is in the array.

There are built-in methods to do all of these things and more!

Some of the more important ones are:

1. `.forEach()`
    * As we saw before, this method calls a function on every value in an array, but will not return a new array with resulting values. 
    * This means that `.forEach()` is a generic tool that should be used in cases where specialized functions, such as the following ones, wouldn't make sense to use.
		<details>
		<summary><b>Example</b></summary>
		<pre>
		var sample = [1, 2, 3];
		sample.forEach(function(elem) {
   			console.log(elem);
		});
		console.log(result);
		/* output */
		[1, 2, 3]
		</pre>
		</details>	
2. `.map()`
    * Map will also call a function on every item in an array, but it will return a new array of resulting values. 
    * This is useful if you don't want to be **destructive**, meaning you don't wan to change the original array.
    	* However, the original array may be changed if the original array is set equal to the resulting array.
    * You will generally use `.map()` to transform an array.
		<details>
		<summary><b>Example</b></summary>
		<pre>
		var sample = [1, 2, 3];
		var result = sample.map(function(elem) {
   			return elem*2; //here we've used map to transform or scale our array by 2.
		});
		/* output */
		[2, 4, 6]
		</pre>
		</details>
3. `.filter()`
    * Filter works like map does: it will iterate over an array and return a new array with the resulting values. 
    * However, it will also filter an array (how could we have ever guessed that??). 
    * Filtering means that only resulting values that return true for a given condition are put into the new array. 
    	* *If the condition is not satisfied (i.e. the value returns false), the element will not be put in the resulting array.* 
    * You will generally use this case to select a subset of multiple elements in an array.
		<details>
		<summary><b>Example</b></summary>
		<pre>
		var sample = [1, 2, 3, 4, 5];
		var result = sample.filter(function(elem) {
   		    if (elem%2 !==0) return elem; //here we've used filter to select only the odd numbers from our array
		});
		console.log(result);
		/* output */
		[1, 3, 5]
		</pre>
		</details>

#### Instructions
1. Practice makes perfect, so let's use all three of these built-in methods heroically.
2. Create an array of the top 5 coolest super powers you can think of. Call this array *superPowers*. In this exercise, you will have all of these super powers (what a dream come true!) 
	<details>
	<summary>Need a Hint?</summary>
	<pre>
	var superPowers = ['super strength', 'super speed', 'invisibility', 'telekinesis', 'telepathy'];
	</pre>
	</details>
3. Use the `.forEach()` method to print out your super powers with its ranking. The ranking would be the index of the item plus 1 (because the first index is always 0). To include the index in your call back function, add another parameter to your function called index. Did it execute as you imagined?
	<details>
	<summary>Need a Hint?</summary>
	<pre>
	superPowers.forEach(function(elem, index) {
		console.log((index+1)+' '+elem);
	});
	</pre>
	</details>
4. Now let’s create an array called *powerPoints*. This array will hold the number of power points you decide each superpower has (it can be completely random). Use the `.map()` function to give your *powerPoints* a boost and multiple each item by 2. Return the array to a new variable called *powerPoints2*. 
	<details>
	<summary>Need a Hint?</summary>
	<pre>
	var powerPoints = [10, 43, 12, 23, 18];
	var powerPoints2 = powerPoints.map(function(elem) {
		return elem*2;
	});
	</pre>
	</details>
5. Oh no! It looks like you’re being attacked by your archenemy. Choose one super power and its corresponding power point to give up. Use `.filter()` to create two new arrays (called *newSuperPowers* and *newPowerPoints*) that don’t include that lost power.
	<details>
	<summary>Need a Hint?</summary>
	<pre>
	var newSuperPowers = superPowers.filter(function(elem) {
		return elem !== ‘invisibility’;
	});
	var newPowerPoints = powerPoints2.filter(function(elem) {
		return elem !== 12;
	});
	</pre>
	</details>
6. Print out your last two arrays to see what your superhero status is. Happy with the results? If not go back into your code and play around with your new best friends: the built-in methods!
7. Continue to [**Conclusion**](../ayesha/exercise5.md)  

