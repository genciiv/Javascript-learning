### What is a variable ?

In programming, a variable is a container for a value .

Your can think of variables as little container for information that live in a computer memory.

Information stored in variables, such as username , account number or even personalized greeting can then be found in memorie

Variables also provide a way of labening data with a descriptive name , so our programs can be understood more clearly by the reader and ourselfs.

In short , variables label and store data in memory.

There are only a few things you can do with variables :

##### - Create a varible with a descriptive name .
##### - Store or update information stored in a variable .
##### - Reference or 'get' information stored in a varible .

#### It is important to distinguish that variables are not values.

They contain values and represent them with a name .

In this lesson , we will cover how to use the var , let , and const keyword to create variables.

### Create a Variable : Var

Create a variable in JavaScript use var keyword like this :

##### var myName = 'Genci';
##### console.log(myName);
##### //Output : Genci

Let's consider this example 
##### var myName = 'Genci';
- var , shot for variable , is a JavaScript keyword that create , or declares a new variable.
- myName is the variable's name . Capitalizing in this way is a standard convention in JavaScript called camel casing. 
In camel casing you group words into one , the first word is lowercase , then every word that follows will have first letter uppercase.
- = is the assigment operator . It assign the value 'Genci' to the variable (myName)
- 'Genci' is a value assigned (=) to the variable myName . You can also say that the myName variable is initialized with a value 'Genci'.
-
### General rules for naming variables
There are few general rules for naming variables :
- Variable name connot start with numbers . 
- Variable names are case sensitive , so myName nad myname would be different variables.
- Variable names cannot be the same as keywords like console , var , ect . For a comprehensive list of keywords check out MDN's keyword documentation.

### Exercise 
- Declare a variable named favouriteFood using the var keyword and assignto it the string 'pizza'.
- Declare a variable named numOfSlices using the var keyword and assign to it the number 8.
- Under the numOfSlices variable , use console.log() to print the value saved to favoriteFood .
- On the following line , use console.log() to print the value saved to numOfSlices.

 ##### var favoriteFood = 'Pizza';
 ##### var numOfSlices = 8;
 ##### console.log(favoriteFood);
 ##### console.log(numOfSlices);


### Create a Variable : let

There were a lot of changes introduced in the ES6 version of JavaScript in 2015 

One of the biggest changes was two new keywords , let and const to create or declare , variables.

The let keyword signals that the variable can be reassigned a differrent value.
Take a look at example 
##### let meal = 'Pizza';
##### console.log(meal); //output : Pizza 
##### meal = 'Burrito';
##### console.log(meal); //Output: Burrito

Another concept that we should be aware of when using let (and even var) is that we can declare a variable without assigned the variable a value.
In such a case , the variable will be automatically initialize with a value of undifined

##### let price;
##### console.log(price); //Output:undifined
##### price = 350;
##### console.log(price); //Output:350

### Exercise 
- Create a let variable called changeMe and set it equal to the boolean true.
- On the line after changeMe is declared , se the value of changeMe to be the boolean false .
- To check if changeMe was reassigned , log the value saved to changeMe to the console.

### Create a Variable : const

The const keyword was also introduced in ES6 , and is short for the word constant.

Just like with var and let you can store any value in a const variable.

The way you declare a const variable and assign a vlaue to it follows the same structure as let and var. Take a lok at the following example.

##### const myName = 'Genci';
##### console.log(myName); // Output : Genci

However , a const variable cannot be reassigned because it is constant .

If you try to reassign a constant variable , ypu will get a TypeError.
Constant variables must be assigned a value when declared. If you try to declare a const variable withpput a value , you will get a SyntaxError.

If you are trying to decide between which keywordto use , let or const think about whether you will neet to reassign the variable latter on.

If you do need to reassign the variable use let , otherwise , use const.

### Exercise
- Create a constant variable named food and set it to equal to the string 'Pizza'
- Just to check that you are saved the value of 'Pizza' to food , log the value of entree to the console.
- Paste the following code to the bottom of your program : food = 'Tacos'
- This code throw the following error when you run your code : TypeError: Assignment to constant variable.





















