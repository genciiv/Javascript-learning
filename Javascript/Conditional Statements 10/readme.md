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

if(true){
    console.log('This code with no run');
}
else{
    console.log('This code will run')
}


##### If . .Else Statements

In the previous exercise we use an if statement that checked a condition to decide wether or not to run a block of code.
In many cases , we will have code we want to run if our condition evaluate to false.
If we wanted to add some default behavior to the if statement , we can add an else statement to run a block of code when the condition evaluate to false.  

An else statement must be paired with an if statement, and together they are referred to as an if...else statement .
In the example above , the else statement :
- Uses the else keyword following the code block of an isstatement
- Has a code block that is wrapped by a set of curlly braces{}
- The code inside the else statement code block will execute when the if statements condition evaluate to false.
- If..else statements allow us to automate solutions to yes or no questions also known, as binary decisions.

##### Exercise 

- Add an else statemen to the existing if statement . Inside the code block of the else statement , console.log() the string "Time to wait to sale"

let sale = true;
sale = false;
if(sale){
    console.log('Time to buy');
}else{
    console.log('Time to wait');
}

#### Comprarison Operators 

When writing conditional statements , sometimes we need to use different type of operators to compare values. These operators are called comparison operators .
Here is a list of some handly comparisons operators and their syntax:

- Less then <
- Greater then >
- Less then or equal to <=
- Greater then or equal to >=
- Is equal to ===
- Is NOT equal to !==

Comparison operators compare the value on the left with the value on the right . For instance:
10<12 // Evaluates to true
It can be helpful to think of comparison statements as questions .

When the answer is "Yes" , the statement evaluates to true , and when the answer is "no" the statement evaluates to false.

The code above would be asking : is 10 less then 12 ? So 10 <12 evaluate to true.

##### Exercise

- Using let , create a variable named hungerLevel and set it equal to 7.
- Write an if ..else statement using a comparison operator 
- The conditional statement should log 'Time to eat' . Otherwise , it should log 'We can eat later'

After you press run , play around with the condition by tweking the comparison of hungerLevel by using different operators such as  <=, >= , > , < , 
































