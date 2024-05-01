1. Line 12 prints `3` because `i` is declared as a `var` and so it can be accessed within the function even outside of the for-block it was declared in. Within the for-loop, `i` iterates until 3, where it stops and exits the for-loop.
2. Line 13 prints `150` because, similar to the previous, `discountedPrice` is a var, and so it can be accessed within the function outside the for-block. Also note that `discountedPrice` saves the last value, which is 300 * (0.5) = 150.
3. Line 14 prints `150` because we have round(150 * 100) / 100 = 150. Also, the code in line 14 is within the scope of `finalPrice`, so it is accessible.
4. The function will return `[ 50, 100, 150 ]` because we declare an array var called `discounted` to be returned, where for each element in `prices`, we calculate the discounted price, round the price, and then push it into `discounted`.
5. The code will cause an error because we use `let` to declare `i` in the for-loop. Thus, `i` is only within scope of the for-block.
6. The code will cause an error because we use `let` to declare `discountedPrice` within the for-loop. Thus, it is only accessible within the for-block.
7. Line 14 will print `150`. The logic follows from question 3. We also note that `finalPrice` was initialized within the function, outside the for-block and line 14 is within the scope of the function.
8. Similar to question 4, the function will return `[ 50, 100, 150 ]`. The same logic applies of initializing an array, calculating the price, rounding the price, pushing them into the array, and then returning the array.
9. The code causes an error similar to question 5 because we declared `i` using `let`, which means that `i` is only in the scope of the for-block.
10. Line 12 will print `3` because we use `length` is defined within the scope of the function, and line 12 is within the function. Also, `length` is initialized to the size of the `prices` array, which is 3.
11. The function will return `[ 50, 100, 150 ]`. The function initializes an array `discounted` and uses a for-loop to iterate through each price in `prices`, where for each price, it calculates the discounted price and pushes it into the `discounted` array. The function returns `discounted`.
12. Given the Object, we write the notation:
    - A. student.name
    - B. student['Grad Year']
    - C. student.greeting()
    - D. student['Favorite Teacher'].name
    - E. student.courseLoad[0]
13. Arithmetic:
    - A. `'32'` because `2` becomes the string '2' in which it gets concatenated to 3. 
    - B. `1` because js will convert `'3'` into the number `3` so that it can subtract it by 2.
    - C. `3` because `null` becomes `0`.
    - D. `'3null'` because `null` will just become the string `'null'` and get concatenated to '3'.
    - E. `4` because `true` maps to 1.
    - F. `0` because both `false` and `null` map to 0.
    - G. `'3undefined'` because `undefined` will become the string `'undefined'` and get concatenated to '3'.
    - H. `NaN` because although `'3'` will be converted to the number `3`, `undefined` does not map to a number, so calculating the subtraction evaluates to Not a Number.
14. Comparison:
    - A. `true` as js will convert `'2'` into a number.
    - B. `false` since both are strings, js will compare Unicode values. (i.e. 50 < 49).
    - C. `true` as js will convert `'2'` into a number.
    - D. `false` since `===` is used, there is no type conversion. So number 2 is not string 2.
    - E. `false` because `true` will map to `1`.
    - F. `true` because `Boolean(2)` will become `true` (i.e. nonzeros evaluate to true). So `===` will be true since both are booleans and the same value.
15. The difference between the == and === operators is that `==` will make type conversions to evaluate value equality, whereas `===` won't and will strictly evaluate type and value equality.
16. See part2-question16.js
17. We start by calling the function with the parameters `[1,2,3]`, an array and `doSomething`, our callback function. Then, `modifyArray` initializes a new array `newArr`. Next, we enter a for-loop, which passes each element in the array into the callback function, which simply multiplies the element by 2. We push this value into `newArr` and then return `newArr` in the end. Thus, we get `[ 2, 4, 6 ]`.
18. See part2-question18.js
19. The output of the code is: `1 4 3 2` because the code will print `1`, then set timeout functions to print `2` after 1 second and `3` after 0 seconds, but does will simultaneously run the code. So `4` immediately gets printed, followed by `3`, and then lastly `2`. 
