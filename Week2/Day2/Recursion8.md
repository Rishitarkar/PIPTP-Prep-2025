

---

###  **Exercise 8 Statement**

> What does the following program compute?

```c
int f(int b) {
    if (b == 0)
        return 1;
    else return g(b, f(b - 1));
}

int g(int a, int b) {
    if (b == 0)
        return 0;
    else return a + g(a, b - 1);
}
```

---

###  **Step-by-step Understanding**

* `g(a, b)` is a **recursive multiplication function**. It computes:

  $$
  g(a, b) = a \times b
  $$

* `f(b)` calls `g(b, f(b - 1))`, and starts from `f(0) = 1`.

So, `f(b)` computes:

$$
f(b) = b \times f(b - 1)
$$

This is the **definition of factorial**!

---

###  **One-Sentence Answer**

**The function `f(b)` computes the factorial of `b`.**

---


