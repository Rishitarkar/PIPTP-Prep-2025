Here’s the full **solution to Exercise 5**, presented right here in the chat:

---

### 🧠 **Exercise 5 Statement**

> Write a recursive function `f` with one positive `int` parameter `n`. The function prints out `2ⁿ − 1` integers in the following pattern:

```
f(1): 1  
f(2): 1 2 1  
f(3): 1 2 1 3 1 2 1  
f(4): 1 2 1 3 1 2 1 4 1 2 1 3 1 2 1  
...
```

> The function does **not** return a value. 4–5 lines of code will do the job.

---

### 🧩 **Pattern Observed**

Each call to `f(n)`:

* Prints `f(n-1)`
* Then prints `n`
* Then prints `f(n-1)` again



---

###  **Recursive Function (Java/C-style pseudocode)**

```java
void f(int n) {
    if (n == 1) {
        System.out.print("1 ");
        return;
    }
    f(n - 1);
    System.out.print(n + " ");
    f(n - 1);
}
```

---

###  **Example Call**

Calling `f(3)` prints:

```
1 2 1 3 1 2 1
```

