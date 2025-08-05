### **Exercise 3: What is returned by `f(5, 3)`?**

Here's the code:

```c
int f(int x, int y) {
    if (y == 0 || y == x)
        return 1;
    return f(x - 1, y) + f(x - 1, y - 1);
}
```

---

###  Observation:

This function is a recursive **binomial coefficient calculator**.
It computes:

$$
f(x, y) = \binom{x}{y}
$$

Why? Because:

* $\binom{x}{0} = 1$
* $\binom{x}{x} = 1$
* Otherwise, $\binom{x}{y} = \binom{x-1}{y} + \binom{x-1}{y-1}$ — Pascal's Rule.

---

###  So, `f(5, 3)` returns:

$$
\binom{5}{3} = \frac{5!}{3!(5-3)!} = \frac{120}{6 \cdot 2} = 10
$$

---

###  **Final Answer: `10`**
