###### BUILT-IN ITERATION METHODS
## The For Loop

##### Go back to [**Introduction**](../ayesha/exercise1.md) 

The way that we've learned how to iterate through an array is the for loop.
The basic template for a for loop is:

```javascript
for (var i = 0; i < array.length; i++) {
   console.log(array[i]);
}
```
Soon we'll look at how to do this in a simpler way, but for now let's refresh our skillz on for loops.

#### Instructions
1. Let's create an array of your favorite superheroes. Create an array of at least 5 strings (I know that choosing your top 5 superheroes can be difficult but try your best). 
	<details>
		<summary>Need a Hint?</summary>
		<pre><code class = "language-javascript">
	var superheroes = ["Batman", "Spiderman", "Wonderwoman", "Black Panther", "Ironman"];
		</code></pre>
	</details>

2. Now let's write a for loop that will iterate through this array to print out our favorite superheroes. Use `console.log()` within your for loop to print out "One of my favorite superheroes is " followed by the superhero you are iterating through.
	<details>
		<summary>Need a Hint?</summary>
		<pre><code class = "language-javascript">
	for (var i = 0; i < superheroes.length; i++) {
		console.log("One of my favorite superheroes is "+superheroes[i]);
	}
		</code></pre>
	</details>

3. Did you see how they printed out a list of all the strings in your array? Did you see how much code you had to write to print that list? Keep both of these in mind for the next exercise.

4. Continue to [**The .forEach() Method**](../ayesha/exercise3.md)  
