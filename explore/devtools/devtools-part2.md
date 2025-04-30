## Question 1

The bug was that the type of `result` was a `string`, rather than a `number`.

## Question 2

I woudld fix it by type-casting the return value of `document.getElementById("num1".value)` and the same for `num2`.