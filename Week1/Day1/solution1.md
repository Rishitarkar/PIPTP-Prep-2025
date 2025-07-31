

###  **Question (Problem Statement)**

Write a function `fun(w, x)` that performs the following:

* Initialize a variable `y` to `0`.
* Check if either:

  * `x` is divisible by `w`, OR
  * `w` is divisible by `x`
* If the condition is true, increment `y` by `1`.
* Otherwise, increment `y` by `10`.
* Print the value of `y` inside the function.
* Call the function with parameters `(40, 4)` and print the return value of the function.

---

###  **Pseudo Code**

```
FUNCTION fun(w, x)
    SET y = 0
    IF (x MOD w == 0) OR (w MOD x == 0) THEN
        y = y + 1
    ELSE
        y = y + 10
    END IF
    PRINT y
END FUNCTION

CALL fun(40, 4)
```

> Note: In the original code, the `fun` function **does not return anything** (i.e., `None` in Python). It only prints `y`. So, `print(fun(40,4))` will print the result of the print inside the function, and then print `None`.

---

###  **Step-by-Step Analysis**

Calling: `fun(40, 4)`

* `w = 40`
* `x = 4`

Check condition:

* `x % w == 0` → `4 % 40 == 4` →  False
* `w % x == 0` → `40 % 4 == 0` →  True

Since one of the conditions is true, the `if` block executes:

* `y = y + 1` → `y = 0 + 1 = 1`

Then:

* Print `1` (inside function)
* Function returns `None` by default (no `return` statement)

So:

* Output from `print(y)` inside function = `1`
* Output from `print(fun(...))` = `None`

---

###  **Final Output on Console**

```
1
None
```


