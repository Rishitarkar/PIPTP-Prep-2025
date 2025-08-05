

---

###  **Exercise 7 Statement**

> Explain in one simple sentence what the following function computes:

```c
int f(int n) {
    if (n == 0)
        return 0;
    if (n % 2 == 0)
        return f(n / 2);
    else
        return 1 + f(n / 2);
}
```

---

###  **Analysis**

This function:

* Divides `n` by 2 recursively.
* Adds 1 **only when `n` is odd**, i.e., when the last bit is `1`.

This is equivalent to **counting the number of 1s** in the **binary representation of `n`**.

---

###  **One-Sentence Answer**

**It returns the number of 1s in the binary representation of `n`.**

---


