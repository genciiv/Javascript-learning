#### Conditional Statements 10

##### What are Conditional Statements 
- In life , we make decisions base on circumstance . If we are tired we go to bed , otherwise we wake up and start our day.
There is-else decisions can be modeled in code by creating conditional statements. A conditional statemen check spicific conditions and performs a task based on th econditions.

##### We will be covering the following conceps :
- if, else if , and else statements
- compariso operators
- logical operators
- truthy and falsy values
- ternary operators
- the switch statement

##### The if keyword

We often perform a task based on a condition . For example , if the weather is niice today , then we will go outside . If the alarm clock rings , then we will shut it off . If we are tired then we wil go to sleep. 
In programming we can also perform a tastk based on condition using an if statement :

if(true){
    console.log(;This message will print);
}

//Prints "This message will print"

  The if statement is composed of :
  - THe if keyword followed by a set of parentheses() which is followed by a code block , or block statement, indicated by a set curly braces{}
  - Iside the paretheses () , a condition is provided that evaluate to true or false . 
  - If the condition evaluates to true , the code inside the curly braces{} runs, or executes
  - If the condition evaluates to false , the block wont execute.

#### Exercise 
- Using the let keyword , declare a variable named sale . Assign the value true on it . 
- Now create an if statement . Provide the if statement a condition of sale . Inside the code block of the if statement , console.log() the String 'Time to buy'
- Below the sale variable declaration, but before the if statement,reassign sale to false . Run your code and observe what happens, we will be changing this behavior i the next exercise.

##### If . .Else Statements

In the previous exercise we use an if statement that checked a condition to decide wether or not to run a block of code.
In many cases , we will have code we want to run if our condition evaluate to false.
If we wanted to add some default behavior to the if statement , we can add an else statement to run a block of code when the condition evaluate to false.  

