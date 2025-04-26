Question 1:

Line 12 will print:
3

This happens because the variable i is declared using var, which is function-scoped; therefore, the variable not limited to just the for loop. Essentially, after the loop finishes running (i = 3 when the loop stops), i still exists and can be used; thus, console.log(i) works (no error) and prints 3.

Question 2:
Line 13 prints:
150

The reason that there is no error is because discountedPrice was declared using var, which makes it accessible throughout the entire function.

Question 3:
At line 14, the code will print the value of finalPrice after the for-loop has finished running. This means it will output the last calculated discounted price from the array. Since finalPrice is updated during each loop iteration and holds a number, there will be no error. Instead, it will simply display the final discounted value based on the last item in the prices array. In this case, it will print 150, because 50% of 300 is 150.

Question 4:
This function will return the array [50, 100, 150]. The reason is that the function takes each price from the input array [100, 200, 300], applies a 50% discount by multiplying by (1 - 0.5), rounds the result to two decimal places, and then adds the final discounted price to the discounted array. After the loop finishes processing all the prices, the function returns the discounted array. There is no error in the code because all variables are properly defined and updated, and the logic correctly handles the discount calculation and array building.

Question 5:
At line 12, the code will cause an error because i is declared using let inside the for-loop, which means i only exists inside the loop block. Outside the loop, i is not defined, so trying to console.log(i) will throw a ReferenceError. In simple words, i is only available inside the loop, and after the loop ends, it disappears, causing an error when trying to use it.

Question 6:
At line 13, the code will cause an error because discountedPrice was declared using let inside the for-loop, so it only exists inside that loop block. Once the loop finishes, discountedPrice no longer exists outside of it. When the code tries to console.log(discountedPrice) after the loop, JavaScript will throw a ReferenceError saying that discountedPrice is not defined.

Question 7:
At line 14, the code will print the value of finalPrice without causing any error. This happens because finalPrice is declared outside the for-loop using let, so it is still accessible after the loop finishes. finalPrice holds the last calculated discounted price, which is 150 (since 50% of 300 is 150), and that value will be printed to the console.

Question 8:
This function will return [50, 100, 150]. It takes the input array [100, 200, 300] and applies a 50% discount to each price by multiplying it by (1 - 0.5), resulting in 50, 100, and 150. Each discounted price is rounded to two decimal places (even though it's not needed here because the numbers are whole), and then added to the discounted array. After the loop finishes, the function returns the discounted array. There is no error because all variables are correctly declared and used within their allowed scope.

Question 9:
At line 11, the code will cause an error because i was declared using let inside the for-loop, so i only exists inside the loop block. After the loop ends, i is no longer available. When the code tries to console.log(i), JavaScript will throw a ReferenceError saying that i is not defined.

Question 10:
At line 12, the code will successfully print 3 to the console without causing any error. This happens because length is declared using const at the top of the function and holds the value prices.length, which is 3 (since the array [100, 200, 300] has three elements). length is in the correct scope and still accessible at line 12.

Question 11:
This function will return [50, 100, 150]. It works by taking each price from the array [100, 200, 300], applying a 50% discount by multiplying each price by 0.5, and then pushing the discounted value into the discounted array. There is no error because all variables are properly declared and used within their correct scopes. After finishing the loop, the function returns the completed discounted array.

Question 12:
A. student.name
B. student['Grad Year']
C. student.greeting()
D. student['Favorite Teacher'].name
E. student.courseLoad[0]

Question 13:
A:
    Output: '32'
    Explanation: The + operator with a string makes JavaScript concatenate the values. The number 2 is converted to a string and joined to '3'.

B:
    Output: 1
    Explanation: The - operator forces JavaScript to convert the string '3' into a number and then subtract. So it becomes 3 - 2 = 1.

C:
    Output: 3
    Explanation: null is treated like 0 in numeric operations. So 3 + 0 = 3.    

D:
    Output: '3null'
    Explanation: The + operator with a string causes string concatenation. null is converted to the string "null", and joined to '3'.

E:
    Output: 4
    Explanation: true is treated like 1 in math. So 1 + 3 = 4.

F:
    Output: 0
    Explanation: false becomes 0 and null becomes 0, so 0 + 0 = 0.

G:
    Output: '3undefined'
    Explanation: The + operator with a string causes string concatenation. undefined becomes the string "undefined" and is joined to '3'.

H:
    Output: NaN
    Explanation: The - operator tries to do math, but '3' is converted to a number 3, and undefined cannot become a number. So the result is NaN (Not a Number).    

Question 14:
A:
    Output: true
    Explanation: JavaScript converts '2' to the number 2, then compares 2 > 1, which is true.

B:
    Output: false
    Explanation: Both are strings, so JavaScript compares alphabetically (like a dictionary). '2' comes after '1', so '2' < '12' is false.

C:
    Output: true
    Explanation: == does type coercion, so '2' is converted to the number 2, and 2 == 2 is true.

D:
    Output: false
    Explanation: === checks for strict equality (no type conversion), and a number (2) is not the same type as a string ('2').

E:
    Output: false
    Explanation: true becomes 1, but 1 != 2, so the result is false.

F:
    Output: true
    Explanation: Boolean(2) is true because 2 is a truthy value. true === true is true.

Question 15: The == operator checks if two values are equal, but it does not care if the types are different. If the types are not the same, JavaScript will try to change one value to match the other before comparing. This is why 2 == '2' is true. On the other hand, the === (strict equality) operator checks if two values are equal and also makes sure they are the same type. It does not change anything. If the types are different, it will return false right away. That is why 2 === '2' is false. In short, == is loose and allows type changes, while === is strict and does not.

Question 16: in js file

Question 17:
The modifyArray function takes the array [1, 2, 3] and applies the doSomething function to each element. doSomething takes a number and returns that number multiplied by 2. So, 1 * 2 = 2, 2 * 2 = 4, and 3 * 2 = 6. Each of these results is pushed into a new array. After the loop finishes, the new array [2, 4, 6] is returned. In short, modifyArray goes through each number, doubles it, and builds a new array with the doubled numbers.

Question 18: in js file

Question 19:
When the function printNums() is called, it first prints 1 immediately because console.log(1) runs right away. Then, setTimeout schedules console.log(2) to happen after 1 second, but it does not run immediately. The next setTimeout schedules console.log(3) with a delay of 0 milliseconds, meaning it will run right after the current code finishes. After setting up these timers, the code moves to console.log(4), which runs immediately and prints 4. Once the main code is done, JavaScript processes the scheduled tasks: console.log(3) happens first because it was scheduled with a delay of 0. Finally, after 1 second, console.log(2) runs. Therefore, the output is 1, 4, 3, 2, in that order.