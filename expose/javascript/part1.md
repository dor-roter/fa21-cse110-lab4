# JS - Part 1
1. *values added: 20*, since `add=true` it will run the if code block add `num1=num2=10` and print result which was saved to `result`
2. *final result: 20*, since `result` is a function scoped variable (declared by `var`), it exists and retains its value outside of the `if` code block.
____
3. *values added: 20*, since `add=true` it will run the if code block add `num1=num2=10` and print result which was saved to `result`
4. The execution will result in an error as `result` is locally declared and it not defined on line 13 (as result of `let`).
____
5. The code will return an error as `result` is a constant variable which is not allowed to be changed (as done at line 7).
6. As an error occured in the previous lines of the function the execution of this functions was not completed thus line 13 did not result in a print.