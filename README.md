# FizzBuzz

FizzBuzz, a program that takes a user's input and prints the numbers from one to the number the user entered.  Numbers that divide by three, five, and three and five, then "Fizz", "Buzz", and "FizzBuzz" are printed.

This is a program that takes a user's input and prints the numbers from one to the number the user entered. However, for numbers that divide by three without a remainder 'Fizz' is printed instead of the number, and for numbers that divide by five without a remainder 'Buzz' is printed. And finally, for numbers that divide by both three and five without a remainder 'FizzBuzz' is printed. 

For example, a typical round of FizzBuzz would start as follows: 

1, 2, Fizz, 4, Buzz, Fizz, 7, 8, Fizz, Buzz, 11, Fizz, 13, 14, Fizz Buzz, 16, 17, Fizz, 19, Buzz, Fizz, 22, 23, Fizz, Buzz, 26, Fizz, 28, 29, Fizz Buzz, 31, 32, Fizz, 34, Buzz, Fizz, ... 

- FizzBuzz is a browser console program, which makes an interface unnecessary. The only user interaction will be allowing users to enter a number. 

- The user enters a number from a prompt (popup box). - The output is a list of numbers from 1 to the number the user enters. But each number that is divisible by 3 outputs 'Fizz', each number that is divisible by 5 outputs 'Buzz', and each number that is divisible by both 3 and 5 outputs 'FizzBuzz'. 

Algorithm in pseudocode:

When a user inputs a number Loop from 1 to the entered number 

If the current number is divisible by 3 then print "Fizz" 

If the current number is divisible by 5 then print "Buzz" 

If the current number is divisible by 3 and 5 then print "FizzBuzz" 

Otherwise print the current number 


First subproblem "user input": 

From this algorithm, the first subproblem to start with is getting input from the user. With JS, a combination of 'parseInt' and 'prompt' will solve the first subproblem. 

let answer = parseInt(prompt("Please enter the number you would like to FizzBuzz up to: ")); 

The above code creates a popup box that asks the user for a number. The prompt call is wrapped in a parseInt function so that a number is returned from the user's input. 

Second subproblem "loop": 

"Loop from 1 to the entered number". 
The for loop will solve this second subproblem. We declare a variable i and assign it 1: the initial value of the variable i in the loop. Due to the needs of this program, we're starting from 1. 

The second clause in the loop is i <= answer - our condition. We want to loop until i is greater than answer. 

The third clause, i++, tells the loop to increment i by 1 every iteration. As a result, if the user inputs 10, the loop would print 1 - 10 to the console. 

for (let i = 1; i <= answer; i++) { 
    console.log(i); } 
    
Here, the first part initializes the loop (the loop starts with 1), the second part checks the condition (the input in this case is 10, and the loop repeats again and again until reaching the input), and the third handles the increment (by each loop iteration the variable i is incremented by 1). 

Like so: for (initialization; condition; finalExpression) {} // loop body