###  **Exercise 4: What is returned by `g(2, 7)`?**

Here’s the function:

```c
int g(int x, int y) {
    if (x == y)
        return x * y;
    return g(x, (x + y) / 2) + g(((x + y) / 2) + 1, y);
}
```

---

###  What's happening?

This function recursively splits the range `[x, y]` into two halves and sums the result of each sub-range.

When `x == y`, it returns `x * y` — i.e., the square of that number.

This acts like a **divide-and-conquer** version of this sum:

$$
g(x, y) = \sum_{i = x}^{y} i \cdot i = \sum_{i = x}^{y} i^2
$$

---

###  For `g(2, 7)`, it computes:

$$
2^2 + 3^2 + 4^2 + 5^2 + 6^2 + 7^2 = 4 + 9 + 16 + 25 + 36 + 49 = \boxed{139}
$$

---

###  **Final Answer: `139`**
