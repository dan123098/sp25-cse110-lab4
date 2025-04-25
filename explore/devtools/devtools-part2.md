# DevTools Part 2: Debugging

## Bug Report and Fix

1. **What was the bug?**  
   The bug was that the values of `num1` and `num2` were being read as strings from the input fields.  
   When the code attempted to add them using `let result = num1 + num2;`, it performed string concatenation instead of numeric addition.  
   For example, `"2" + "3"` resulted in `"23"` rather than `5`.

2. **How would you fix it?**  
   Convert the input values to numbers before performing the addition.  
   Here's the corrected line of code:

   ```js
   let result = Number(num1) + Number(num2);
   ```

---

**Screenshots to include (place in `expand/screenshots/`):**
- `result-calculateSum.png`: Breakpoint set at the result line in `calculateSum()`
- `result-dataType.png`: Watch expressions showing `num1`, `num2`, and `typeof result`
- `fix.png`: Screenshot of the fixed code
