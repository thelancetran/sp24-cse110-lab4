1. Line 9 prints: `values added: 20`
2. Line 13 prints: `final result: 20`
3. Line 9 prints: `values added: 20`
4. The code returns an error because `result` has a **block scope**, in which it can only be accessed within the if-block. Line 13 is outside of this block, so it cannot access `result`.
5. The code returns an error because `result` is a const and so it's value cannot be reassigned. Thus, in line 7 when we try to change `result`, we get a TypeError.
6. Similarly, the code returns an error because it tries to reassign `result` when it is a declared as a `const`.
