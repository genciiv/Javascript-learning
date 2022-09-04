### Mathematical Assignment Operators

Let's consider how we can use variables and math operators to calculate new values and assign them to a variable.
Check out the example below :

##### let a = 4;
##### a = a + 1;
##### console.log(a); // Output:5

In example above , we created the variable a with the number 4 assigned to it .
The following line , a = a + 1 , increases the value of from 4 to 5.

- Another way we could have reassigned a after performing some mathematical operation on it is to use buil-in mathematical assignment operators.
We could re-write the code above to be :

##### let a = 4;
##### a+ = 1;
##### console.log(a); //Output : 5

In second example , we used the +=assignment operator to reassign w. We are performing the mathematical operation of the first operator .
+ using the number to the right , then reassignning a to the computed value.

- We also have access to other mathematical assignment operators : -= , *= , and /= .
which work in a similar fashion .
##### let x = 20;
##### x -= 5; // Can be written as x=x-5
##### console.log(x); // Output : 15

##### let y = 50;
##### y *= 2; // Can be written as y = y * 2 
##### console.log(y); // Output : 100

##### let z = 8;
##### y /= 2; // Can be written as z = z / 2 
##### console.log(y); // Output : 4


### Exercise 

- Use the += mathematical assignment operator to increase the value stored in levelUp by 5.
- Use the -= mathematical assignment operator to decrease the value storedd in powerLevel by 100.
- Use the *= mathematical assignment operator to multiply the value stored in multiplyMe by 11.
- Use the /=  mathematical assignment operator to devide the value stored in quarterMe by 4.

### The Increment and Decrement Operator 
Other mathematical assignment operators include the increment operator (++) and decrement operator (--).
The increment operator wil increase the value of the variable by 1. The decrement operator will decrease the value of the variable by 1 . For example .

##### let a = 10;
##### a++;
##### console.log(a); //Output : 11

##### let b = 20;
##### b--;
##### console.log(b); // Output : 19

Just like the previous mathematical assignment operators(+=,-=,*=,/=) the variable's value is updated and assigned as the new value of that variable.

### Exercise 
- Using the increment operator , increase the value of gainedDollar.
- Using the decrement operator, decrease the value of lostDollar.

## String Concatenation with variables 
In previous exercise , we assigned strings to variables . Now let's go over how to connect , or concatenate , stringsin variables.

The + operator can be used to combine two string value even if those values are beign stored in variables :
##### let myPet = 'Beny';
##### console.log('I own aa pet' + myPet); // Output I own a pet Beny


### Exercise 
- Create a variable named favoriteAnimal and set it equal to your favorite animal.
- Use console.log() to print 'My favorite Animal' to the console . Use string concatenation so that Animal is replaced with the value in your favoriteAnimal variable.

##### let favoriteAnimal = 'Cat';
##### console.log('My favorite animal is' + favoriteAnimal);


### String Interpolation 

In the ES6 version of JavaScript , we can insert , or interpolate , variables into strings together.

Check out the following example where a template literal is used to log strings together .

##### const myPet = 'Lucky';
##### console.log('I own a pet ${myPet}.');
##### // Output : I own a pet Lucky

### Notice that :

- a template literal is wrapped by backticks 'this key usually located on the top of your keyboard , let of the 1 key'.
-Inside the template literal , you will see the placeholder , ${myPet} The value of myPet is inserted into the template literal.
- When we interpolate 'I own a pet ${myPet}' the output we print is the string 

One of the biggest benefits to using template literal is the readability of the code 
Using template literals , you can more easily tell what the new string will be.
You also dont have to worry  about escaping double quotes or single quotes.

### Exercise 

- Create a variable called myName and assign it your name.
- Create a variable called myCuty and assign it your favorite city's name.
- Use a single template literal to interpolate your variables ito the sentece below.
- Use console.log() to print your sentence to the consolein the following format.
- My name is Name . My favorite city is CITY

- Repalce Name and CITY in the string above by interpolating the values saved to myName and myCity.
 
let myName = 'Genci';
let myCity = 'Fier';
console.log('My name is ${myName}. My Favorite city is ${myCity}.');


### Typeof operator 

While writing code , it can be useful to keep truck of the data types of the variables in your program.
If you need to check the data type of variable's alue , you can use the typeof operator.
The typeof operator checks the value to its tight and returns or passes back a string of the data type.

const unkwown1 = 'foo';
console.log(unkwown1); // output string

const unknown2 = 10;
console.log(unknown2); // output number

Let's break down the first example . Since the value unknown1 its 'foo' a string unknown1 will return 'string'.



