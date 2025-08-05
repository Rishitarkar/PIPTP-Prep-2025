
 ** C++ / Java-style pseudocode:**

```java
int sumDigits(int x) {
    if (x == 0)
        return 0;
    return (x % 10) + sumDigits(x / 10);
}
```

###  Explanation:

* Base case: If `x == 0`, return 0.
* Recursive case: Take the last digit using `x % 10` and add it to the result of `sumDigits(x / 10)` (the number with the last digit removed).

###  Example:

For `x = 456`, the call trace will be:

```
sumDigits(456) = 6 + sumDigits(45)
               = 6 + 5 + sumDigits(4)
               = 6 + 5 + 4 + sumDigits(0)
               = 6 + 5 + 4 + 0 = 15
```

Let me know if you'd like solutions for Exercises 3 and 4 as well.
