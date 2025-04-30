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

## Question 13

A. Output: `'32'`. The environment sees the `+` operator and a string and an integer on either side. It prioritizes the conversion of the integer to a string, and thus concatenates `'3'` and `'2'` to make `'32'`

B. Output: `1`. The environment see the `-` operator, and thus ensures both operands are numbers or, in this case, integers. We perform `3 - 2` which is `1`.

C. Output: `3`. The environment sees the `+` operator, an integer operand, and a `null`. It converts `null` to the integer `0`, and performs `3 + 0` which is `3`.

D. Output: `'3null'`. The environment sees the `+` operator and at least one string as an operand, treating the operation as concatenation. This converts `null` to `'null'` and performs `'3' + 'null' = '3null'`.

E. Output: `4`. The environment treats the operator as addition and converts `true` to `1`, performing `1 + 3 = 4`.

F. Output: `0`. The environment defaults to integer operation, converting both `false` and `null` to `0`, performing `0 + 0 = 0`

G. Output: `'3undefined'`. Because one of the operands is a string, and the operator is `+`, we perform concatention and convert `undefined` to a string.

H. Output: `NaN`. The `undefined` keyword becomes `NaN` with operations other than `+`, and `'3' - 'NaN'` produces an string error, resulting in `NaN` as the output.

## Question 14

A. Output: `true`. The `'2'` string converts into an integer, and `2 > 1` is a true statement.

B. Output: `false`. We perform string comparisons by lexicographical order. Since `'2'` comes after `'1'`, the statement is false.

C. Output: `true`. We convert `'2'` to the integer `2`. The statement `2 == 2` is true.

D. Output: `false`. We perform a strict equality operation. Since our operands are different types (string and integer), we return false.

E. Output: `false`. We convert `true` to the integer `1`. The statement `1 == 2` is false.

F. Output: `true`. We explicitly convert the integer `2` into the boolean `true` since it is non-zero. Thus, `true === true` is true.

## Question 15

The difference between the regular equality operator `==` and the stric equality operator `===` is that the former perfroms type conversions, while the latter does not. Once the strict equality sees that it is comparing two operands of different types, it automatically returns false. However, with regular equality, it may perform type conversions and the result may end up being true.

## Question 16

*Solution in part2-question16.js*

## Question 17

The result of `modifyArray([1,2,3], doSomething)` is a new array with double the values of the original: `[2, 4, 6]`. In the `modifyArray` function, first we create a new array `newArr`. Then in a for loop, we iterate through each entry in the array, and pass it as an argument into the `doSomething` function. This doubles the value and returns the result, and then pushes the value into the `newArr`. Finally, the function returns this array of double values.

## Question 18

*Solution in part2-question18.js*

## Question 19

The output of the code is `1 4 3 2`. The 1 and 4 get printed out immediately, since they are on the original callstack. Then, 3 prints out immediatly after, and then 2 gets printed after 1 second.