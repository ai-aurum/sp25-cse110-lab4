## Question 1:

Line 9 prints `values added: 20` since `add` is true and the sum of 10 and 10 is 20, which is stored in `result`. Additionally, `result` was declared in the same scope as the print function, so there is no error.

#

## Question 2:

Line 13 prints `final result: 20`. There is no error here since `result` was declared using the `var` keyword, making it global.

#

## Question 3:

You should not use `var` because it ignores code blocks and has global access. A consequence of this naming issues. For example, a variable `var x` may be declared in a function, but still exists in the Lexical Environment. As a result, one might run into the issue of trying to create another variable with the same name `x`. Additionally, variables declared with `var` might be unintentionally modified by another part of the source code.

#

## Question 4:

Line 9 prints out `values added: 20`, just like before.
 
#

## Question 5:

Line 13 now prints an error, since the `result` variable does not exist within the scrop of this print statement. This is because the variable was declared with the `let` keyword, in which the variable's scope is only within the code block it was defined in.

#

## Question 6:

Nothing is printed on line 9, since line 7 throws an error. This error is the result of attempting to reassign the value of a `const` variable, specifically `result` which was initialized to 0 on line 5.

#

## Question 7:

For the same reasons as Question 6, line 13 does not print anything. Even if there was not an assignment error, the `result` variable is still not in the same scope as the print statment on line 13.


