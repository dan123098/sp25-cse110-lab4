# Part 2 Answers

### Question 12
A. `student.name`  
B. `student["Grad Year"]`  
C. `student.greeting()`  
D. `student["Favorite Teacher"].name`  
E. `student.courseLoad[0]`

---

### Question 13 - Arithmetic
A. '3' + 2 → `"32"` (string concatenation)  
B. '3' - 2 → `1` (`'3'` coerced to number)  
C. 3 + null → `3` (`null` becomes 0)  
D. '3' + null → `"3null"` (string concatenation)  
E. true + 3 → `4` (`true` becomes 1)  
F. false + null → `0` (`false` → 0, `null` → 0)  
G. '3' + undefined → `"3undefined"` (string concatenation)

---

### Question 14 - Comparison
A. '2' > 1 → `true`  
B. '2' < '12' → `false` (string comparison)  
C. 2 == '2' → `true` (type coercion)  
D. 2 === '2' → `false` (strict equality)  
E. true == 2 → `false`  
F. true === Boolean(2) → `true` (both are `true` boolean)

---

### Question 15
**Difference between == and ===:**  
`==` compares values with type coercion.  
`===` compares both value and type (strict equality).

---

### Question 16
```js
for (let key in statistics) {
  if (key.startsWith('r') || statistics[key] % 2 === 1) {
    console.log(statistics[key]);
  }
}
```

---

### Question 17
**Output:** `[2, 4, 6]`  
**Why:** Each value in `[1, 2, 3]` is passed to `doSomething`, which doubles it, and the result is pushed to the new array.

---

### Question 18 - part2-question18.js
```js
setInterval(() => {
  let d = new Date();
  let time = d.toLocaleTimeString();
  console.log(time);
}, 1000);
```

---

### Question 19
**Output:**  
```
1  
4  
3  
2
```
**Why:**  
- `console.log(1)` runs first.  
- `console.log(4)` runs immediately after.  
- `console.log(3)` is delayed by 0 ms (runs right after current stack is empty).  
- `console.log(2)` is delayed by 1000 ms.
