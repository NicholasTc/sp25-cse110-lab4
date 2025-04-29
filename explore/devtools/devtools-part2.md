Question 1:
The num1 and num2 values retrieved from the DOM are strings, not numbers.
So, when the calculateSum() function adds them with num1 + num2, it performs string concatenation instead of numeric addition.

Question 2:
Because the main issue is that the variables are strings due to DOM retrieval, the solution is to parse those variables using Number to convert string to integer; therefore, the calculations are now correct (no longer concatenation)