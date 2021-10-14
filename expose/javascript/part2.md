# JS - Part 2
1. since `i` was declared by the keyword `var` it is part of the functions scope and will be prinited out with its most recent value - `3`
2. since `discountedPrice` was declared by the keyword `var` it is part of the functions scope and will be prinited out with its most recent value - `150`
3. since `finalPrice` was declared by the keyword `var` it is part of the functions scope and will be prinited out with its most recent value - `150`
4. An array with the discounted prices - each price in prices will be cut down by 50% and rounded up to 2 decimal positions.
5. as `i` is now declared by `let` it exists only within the `for`'s scope, thus accessing it on line 12 results in an exception (access of undefined variable).
6. as `discountedPrice` is now declared by `let` it exists only within the `for`'s scope, thus accessing it on line 12 results in an exception (access of undefined variable).
7. Although `finalPrice`  is declared using the keyword `let` it is declared in the function's "main" scope which is the very same scope of line 14, thus it will result in printing the latest value saved in `finalPrice` - 150
8. An array with the discounted prices - each price in prices will be cut down by 50% and rounded up to 2 decimal positions.
9. Although `discounted` is declared as const pushing elements into an array is allowed and as such the `for` loop execution will complete reaching line 11 where similarly to question 5 will result in an error. 
10. Same as last question for the  `for` loop, and then accessing `length`  is allowed and so the execution completes and `3` is printed.
11. As described above, the function will complete its executions and will result in returned array with prices cut down by 50% (not rounded to 2 decimal points).
## Data Types
___
12. 
    1.  ```
        student.name
        ```
    2.  ```
        student['Grad Year']
        ```
    3.  ```
        student.greeting()
        ```
    4.  ```
        student['Favorite Teacher'].name
        ```
    5.  ```
        student.courseLoad[0]
        ```
## Basic Operators & Type Conversion 

___
13. 
    1. `32` since integers map to their exact string representation
    2. `1` since '3' becomes a number
    3. `3` since null=0
    4. `3null` null toString is "null"
    5. `4`  since true maps to 1
    6. `0` since both false and null numerically equal 0
    7. `3undefined` undefined toString is "undefined"
    8. `NaN` undefined is Nan as a number
14. 
    1. `true` '2' becomes 2
    2. `false` lexicographical ordered as both are strings
    3. `true` '2' is casted to 2 
    4. `false` as the two are not exactly identical (different types)
    5. `false` true is 1 numerically
    6. `true` non-zero number in boolean is true
15. == ignores datatypes and makes the necessary conversions before comparing but === comapres while checking the datatypes.
## Functions
______

17. The function applies the callback "element-wise" on the provied array same as `map` and then returns the newly mapped array. Thus, `[1,2,3]` will be transformed into `[2,4,6]`.
## setInterval(), setTimeout(), clearTimeout()
___
19. ```
    1
    4
    3
    2
    ```
    first sync code will be executed in order then the event loop will free up and schedule the first ready timeout callback then the second resulting in the order listed above.
