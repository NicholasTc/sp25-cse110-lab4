
Question 1: 
There is no error when I execute the code and it prints:
values added:  20

There is no error because result is declared using "var", which is function-scoped, not block-scoped. This means result is accessible throughout the entire sumValues function—even outside the if block. In this case, using "var", "let", or "const" technically does not matter because we are running console.log in the same scope which is the if block; thus, it will run just fine. 

Question 2:
There is also no error and the output is:
final result:  20

Similar to the previous reasoning, the reason that there is no error because result is declared using var, which is function-scoped. This means that result is accessible throughout the entire sumValues function, including both inside and outside the if block. However, if we declare the value with "let" or "const" it will throw out a reference error because there is a reference error because let and const are block-scoped, so variables declared inside the if block are not accessible outside of it.

Question 3:
We should always avoid using var because it is function-scoped, not block-scoped, so even if you declare it inside an if or for block, or some other block, it still exists outside that block. This can lead to unexpected behavior and make your code harder to understand or debug; specifically, it can lead to scoping and conflict issues. 

Instead, we should always use let or const because they are block-scoped, which means the variable only exists where it’s supposed to. This makes the code more secure

Question 4:
Line 9 prints:
values added:  20

There is no error because the variable "result" is declared using let inside the if (add) block, and line 9 is also inside that same block. Essentially, the variable is accessible and works fine; thus, no error occurs.

Question 5:
Upon executed line 13 will output:
ReferenceError: result is not defined

The reason for the error is that the variable "result" was declared with let inside the if block, which means it is block-scoped. Moreover, line 13 is outside that block, so it cannot access result, leading to a ReferenceError. In other words, this is a scoping issue. 

Question 6:
Line line will output:
TypeError: Assignment to constant variable.

The reason for that is because on line 5, result is declared using const, which means it cannot be reassigned after its initial value (0). However, line 7 attempts to reassign "result=num1 + num2". Const does not allow for reassign.

Question 7:
Upon running line 13, the error does not explicitly printed because we have the previous reassign issue from line 9. However, line 13 will output "ReferenceError: result is not defined" because const has the same scope as let; therefore, result is not accessible outside the if block. 

