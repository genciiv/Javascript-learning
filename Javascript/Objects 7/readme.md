## Built-in Objects

In addition to console , there are other objects built into JavaScript .
Down the line you will build your own objects, but for now these 'build-in' objects are full of usefull functionally.

For example , if you want to perform more complex mathematical operation then arithmetic , JavaScript has the buil-in Math object.

The great thing about objects is that they have methods ! Let's call the random() method for the built-in Math object:

console.log(Math.random()); // prints a random number between 0 and 1

In example above , we called the .random() method by appending the object name with the dot operator, the name of the method ,
and opening and closing parentheses. 
This method returns a random number between 0 and 1.

##### To generate a random number between 0 and 50 , we could multiply this result by 50, like so :

Math.random()*50;

The example above will likely evaluate to a decimal .
To ensure the answer is a whole number , we can take advantage of another useful Meth method called Math.floor()

console.log(Math.floor(Math.random()*50)); // prints a whole number


In this case :

Math.random generates a random number between 0 and 1.
We then multiply that number bby 50 , so now we have a number between 0 and 50 .
The , Math.floor() rounds the number down to the nearest whole number .

### Exercise

Inside of a console.log(), create a random number with Math.random() , then multiply it by 100

console.log(Math.random()*100)

### Exercise 

Use Math.florr() to make the output a whole number .
Inside the console.log you wrote in the last step , put Math.random()*100 inside the parentheses of Math.floor

console.log(Math.floor(Math.random()*100));

### Exercise 

Find a method on the JavaScript Math object that runs the smallest integer greater then or equal to a decimal number .
Use this method with the number 43.8. Log the answer to the console.

console.log(Math.ceil(43.8)); // prints 44
