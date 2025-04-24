# Part 1 Answers

### Question 1
**Output (line 9):** values added: 20  
**Why:** The `add` parameter is `true`, so the block executes. `var` is function-scoped and accessible throughout the function.

### Question 2
**Output (line 13):** final result: 20  
**Why:** `var` allows access outside of the if block.

### Question 3
**Why not use `var`:** Because `var` is function-scoped and can lead to unexpected behavior. It allows redeclaration and hoisting, which can introduce subtle bugs.

---

### Question 4
**Output (line 9):** values added: 20  
**Why:** `let` is block-scoped, but we're inside the same block.

### Question 5
**Output (line 13):** ReferenceError  
**Why:** `result` is block-scoped due to `let`, so it's not accessible outside the `if` block.

---

### Question 6
**Output (line 9):** TypeError  
**Why:** You can't reassign a `const` variable after declaration.

### Question 7
**Output (line 13):** Not reached due to error on line 9

---

### Question 8
**Output:** [50, 100, 150]  
**Why:** Each item is multiplied by 0.5 and pushed into `discounted`.

### Question 9
**Output (line 11):** ReferenceError  
**Why:** `i` is block-scoped with `let` and not accessible outside the loop.

### Question 10
**Output (line 12):** 3  
**Why:** `length` is declared with `const` and still in scope at line 12.

### Question 11
**Output:** [50, 100, 150]  
**Why:** The function calculates 50% off each number and returns the new array.
