# Part 2

## Question 1

At line 12, we print out the value `i` which is 3. This is because the `prices` list passed as an argument has length 3, and the `for` loop dependent on the counter variable `i` runs for as long as the length of the list argument. Even though the variable was declared in the `for` loop block, it was declared using the `var` keyword, thus there is still global access to it and we can print out its value without problem.

## Question 2

At line 13, we print out the discounted price of the last element in our `prices` list, which is 150. We are allowed access to the value of `discountedPrice` because it was declared using the `var` keyword. Also, the most recent value of `discountedPrice` is when `i = 2`, and thus `prices[2]` is the last element in the list. When applying the discount operations, we yield the value of 150.

## Question 3

At line 14, we print out `finalPrice`, which is 150. Regardless of how this variable was declared i.e. with `var` or `let`, we are able to print out its value without problem, since the variable and the print statement are within the same scope. By line 14, `finalPrice` holds the discounted price of the last item in our `prices` list, similar to Question 2.

## Question 4

This function will successfully return a list of the discounted prices that were passed as the argument. That is, `[50, 100, 150]`. More specifically, it returns a reference to the data that `discounted` held.

## Question 5

At line 12, the code throws an error. This is because `i` does not exist in the scope of the print statement, since `i` only existed within the `for` loop, determined by the `let` declaration of `i`.

## Question 6

Similar to Question 5, line 13 will throw an error, since the `discountedPrice` variable does not exist within the scope of the print statement. Because of the `let` declaration of this variable, it only existed in the `for` loop block it was declared in.

## Question 7

As mentioned in Question 3, we can print out the `finalPrice`, 150, without problem, since this variable was declared within the same scope of the print statement. In this case, it would not have mattered if we used `var` or `let`.

## Question 8

This function will successfully return a list of the discounted prices, similar to Question 4. The function does not rely on a global scope to access its variables, and thus behaves similar to the function with `var` variable declarations.

## Question 9

At line 11, the code throws an error, since `i` is undefined within the scope of the print statement. Because it was declared with `let`, it only exists within the `for` loop.

## Question 10

At line 12, we are able to print out the value of `length`, 3, without problem. This is because `length` was declared within the same scope as the print statement on line 12.

## Question 11

This function returns the same list of discounted prices as previous version of the functions have: `[50, 100, 150]`. No `const` variables were reassigned a different value, and no other variables were accessed outside of their scope. Thus, there were no errors in the code.

## Question 12

A. `student.name` \
B. `student['Grad Year']` \
C. `student.greeting()` \
D. `student['Favorite Teacher'].name` \
E. `student.courseLoad[0]`
