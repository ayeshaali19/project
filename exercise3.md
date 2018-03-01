###### BUILT-IN ITERATION METHODS
## The forEach Built-In Method

##### Go back to [**The For Loop**](../ayesha/exercise2.md) 

The `.forEach()` method does the same repetition that the for loop does.
The basic template for the `.forEach()` method is:

```javascript
   array.forEach(function(item) {
      console.log(item);
   });
```
This method works by taking in a function as a parameter whereas in a for loop any functions used or actions done is put in the body of the loop. In this example, the function is called on each item in the array and prints those values. 

#### Instructions
1. Let's take another look at your array of superheroes. 
2. Now let's use the `.forEach()` method to iterate through this array to print out your superheroes. Use `console.log()` again to print out "One of my favorite superheroes is " followed by the superhero.
	<details>
		<summary>Need a Hint?</summary>
		<pre><code class = "language-javascript">
	superheroes.forEach(function(superhero) {
		console.log(superhero);
	});
		</code></pre>
	</details>

3. Feeling a bit of déjà vu yet? Because we are.
3. Feeling a bit of déjà vu yet? Because we are.
4. The for Loop and the `.forEach()` method execute the same way! 
5. But why is this built-in method even useful if we have the for loop? To find out, continue to [**Simpler Is Better**](../ayesha/exercise4.md)  

