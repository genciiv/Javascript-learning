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








