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

let hungerLevel = 7;
if(hungerLevel<=7){
    console.log('Time to eat');
}else{
    console.log('Time to wait');
}

##### Logical Operators

Working with conditionals means that we will be using booleans , true or false values.
In javascript , there are operators that work with boolean values known as logical operators .
We can use logical operators to add more sophisticated logic to our conditionals.
There are three logical operators :

- The and operator (&&)
- The or operator (||)
- The not operator , otherwise known as the bang operator (!)

###### When we use the && operator , we are checking that two things are true

let stopLight ='green';
let pedestrians = 0;

if (stopLight === 'green' && pedestrians===0){
    console.log('GO!')
}else{
    console.log('Stop')
}

###### When using the && operator , both conditions must evaluate to true for the entire condition to evaluate to true and exucute.

If we only care about either condition begin true , we can use the || operator

if(day==='Saturday' || day==='Sunday'){
    console.log('Enjoy the weekend');
}else{
    console.log('Do some work')
}

When using the || operator , only one of the conditions must evaluate to true for the overall statement to evaluate to true. In the code example above , if either day==='Saturday' or day===='Sunday' evaluate to true the ifs condition will evaluate to true and its code block will execute . The code in the else statement above will execute only if both comparisons evaluate to false.


###### The ! not operator reverses , or negates , the value of a boolean

let excited = true;
console.log(excited) // Prints false

let sleepy = false;
console.log(sleepy); //Prints true

Essentially the ! operator will either take a true value and pass back false , or it will take a false value and pass back true.
Logical operators are often used in conditional statements to add another  layer of logic to our code

let excited = true;

if(!excited){
    console.log('I am exited');
}else{
    console.log('I am not exited');
}

### Exercise

- Declare two variab;es mood='sleepy' and tirednessLevel=5.
- Lets create an if....else statement that check if mood is sleepy and tirednessLevel is greater then 8.

-If both conditions evaluate to true , then console.log() the string 'Time to sleep' . Otherwise , we should console.log() 'not bed time yet'
-After your press "Run" , play around with the || operator and the ! operator ! What happens if you negate the value of the entire statement with ! and switch to || instead of &&

let mood = 'sleepy';
let tirednessLevel = 5;

if(!(mood==='sleepy' && tiredlessLevel >8)){
    console.log('time to sleep');
}else{
    console.log('not bed time yet');
}

#### Truthy and Falsy

Lets consider how non-boolean data types , like strings or numbers are ealuated when checked inside a condition.

Sometime you will want to check is a variable exists and you want necessarily want it to equal a specific value - you will only check to see if the variables has been assigned a value.

let myVariable = 'I Exist';
if(myVariable){
    console.log(myVariable)
}else{
    console.log('The variable does not exist')
}



let myVar; // =value;
if(myVar){
    console.log(myVar);
}else{
    console.log('The variable is not initialized')
}

The code block in the if statement will run because myVariable has a truthy value even through the value of myVariable is not explicitly the value true , when used in boolean or conditional context, in evaulates to true because it has been assigned a non-falsy value.

So which values are falsy - or evaulate to false when checked as a conditional > The list of falsy values includes:
- 0
- Empty string like "or"\null which represent when there is no value at all
- undefined which represent when a declared variable lacks a value 
- NaN or Not a Number

Below checks if username is defined and assigns a defaultstring if it is not:

let defaultName;
if(username){
    defaultName = username;
}else{
    defaultName = 'Stranger';
}

If you combine your knowledge of logical operators you can use a short-hand for the code above. In a boolean condition , JavaScript assigns the truthy value to a variable if you use the || operator in your assignment:

let defaultName = username || 'Stranger'

Because || or statments check the left-hand condition first , the variable defaultName will be assigned the actual value of username if it is truthy and it will be assigned the value of 'Stranger' if username is falsy. This concept is also referred to as short-circuit evaluation.

let username;
let defaultName;
if(username){
    defaultName = username;
}else{
    defaultName = 'Stranger';
}
console.log(defaultName);


### Ternary Operator

In the spirit of using short-had syntax we can use a ternary operator to simplify an if...else statment

Take a look at the if...else statment example :

let isNightTime=true;
if(isNightTime){
console.log('Turn on the light');
}else{
console.log('Turn off the light');
}

In the example above "
- The condition isNightTIme is provided before the ?
- Two expressions follow the? and are separated by a colon :
- If the condition evaluates to true , the first expression executes
- If the condition evaulate to false , the second expression executes

let stopLight = yellow;

if(stopLight==='red'){
    console.log('Stop');
}else if(stopLight==='yellow'){
    console.log('Slow down');
}else if(stopLight==='green'){
    console.log(Go);
}else{
    console.log('Caution,unknow');
}

























