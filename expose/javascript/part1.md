## Question 1:

Line 9 prints `values added: 20` since `add` is true and the sum of 10 and 10 is 20, which is stored in `result`. Additionally, `result` was declared in the same scope as the print function, so there is no error.

## Question 2:

Line 13 prints `final result: 20`. There is no error here since `result` was declared using the `var` keyword, making it global.

## Question 3:

You should not use `var` because it ignores code blocks and has global access. A consequence of this naming issues. For example, a variable `var x` may be declared in a function, but still exists in the Lexical Environment. As a result, one might run into the issue of trying to create another variable with the same name `x`. Additionally, variables declared with `var` might be unintentionally modified by another part of the source code.

