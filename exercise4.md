###### BUILT-IN ITERATION METHODS
## Simpler Is Better

##### Go back to [**The forEach Built-In Method**](../ayesha/exercise3.md)  

Now that we've looked at both the for loop and `.forEach()`, these two methods need to battle it out to see which one is the better choice. Let's look at the pros and cons of any built-in method.

### Pros
1. The built-in method is **more readable** 
	* The choice of a built-in method shows the purpose of the loop, thus making it more understandable.
	* In the case of `.forEach()` we want to iterate through an array (without creating a new one, but more on this later).
2. The built-in method is **less boilerplate**
	* Boilerpater sections of code mean are sections of many lines of code that is needed to do a relatively simple task. 
	* Writing for loops is considered boilerplate; it is unnecessarily long and can distract from the actual intention of the code. Using the built-in method solves this problem.
3. The built-in method provides **less room for error**
	* Using a built-in method ensures the loop will  work as you want it to, whereas a for loop is prone to typos that can mess up all your code.
4. The built-in method ensures **less scope issues** 
	* Each for loop declares a variable for its loop. This variable enters the function's scope, adding unnecessary values and potentially overwriting existing variable values.
	* This problem is called scope pollution, which is not an issue with built-in methods. 

### Cons
1. The for Loop does **run faster** than let's say the `.forEach()` method. However, that usually does not matter because the difference is generally minute. 

#### Instructions
1. `console.log()` the answer to this question: Is it better to use built-in methods over for loops?
	<details>
		<summary>Need a Hint?</summary>
		<pre>The answer is yes!</pre>
	</details>
2. Continue to [**Other Built-In Methods**](../ayesha/exercise5.md)  
