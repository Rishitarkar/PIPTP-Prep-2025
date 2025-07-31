<img width="1098" height="505" alt="Screenshot 2025-07-31 at 1 48 04 PM" src="https://github.com/user-attachments/assets/181a09be-7474-49c1-be43-f6b34e77b909" />
Let's analyze the pseudocode with inputs `a = 4` and `b = 3`:

---

###  Pseudocode Summary:

```text
function funn(a, b):
  if a > 0:
    return funn(a-2, a+b) + funn(a-3, a+b) + funn(a-4, a+b)
  else:
    a = b
    b = a
    return a + b
```

So the **base case** is when `a <= 0`, it returns `a + b` (which becomes `2*b` since `a = b` and `b = a`).

---

###  compute `funn(4, 3)` step-by-step:

**Step 1: funn(4,3)**
→ `a > 0`, so:

```
= funn(2,7) + funn(1,7) + funn(0,7)
```

---

###  Compute `funn(2,7)`

```
= funn(0,9) + funn(-1,9) + funn(-2,9)
```

* `funn(0,9)` → base case → return `2*9 = 18`
* `funn(-1,9)` → base case → return `18`
* `funn(-2,9)` → base case → return `18`

➡ Total: `18 + 18 + 18 = 54`

---

###  Compute `funn(1,7)`

```
= funn(-1,8) + funn(-2,8) + funn(-3,8)
```

* All are base cases → return `16` each

➡ Total: `16 + 16 + 16 = 48`

---

###  Compute `funn(0,7)`

→ base case → return `2 * 7 = 14`

---

###  Final Answer:

```
funn(4,3) = 54 + 48 + 14 = 116
```

---

### ✔ Correct Option: **A. 116**
