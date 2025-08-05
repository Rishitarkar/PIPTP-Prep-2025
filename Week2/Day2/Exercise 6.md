
---

###  **Exercise 6 Statement**

> Write a recursive function that takes a **positive integer** and returns the **number of 1’s** in the **binary representation** of that integer.

---

###  **Concept**

To count the number of 1s in the binary representation of a number `n`, we can:

* Check the last bit using `n % 2`
* Recursively process the remaining bits using `n / 2`

---

###  **Recursive Function (Java/C-style pseudocode)**

```java
int countOnes(int n) {
    if (n == 0)
        return 0;
    return (n % 2) + countOnes(n / 2);
}
```

---

###  **Example: `countOnes(13)`**

* Binary of 13 = `1101`
* Number of 1s = 3
   Output: `3`

---


