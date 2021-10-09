# pyfuck
One line Brainfuck interpreter in Python

### Note
The implementation don't use
  - `+`, `-` (only to do `-1`, etc...), `<`, `>`, etc...;
  - No keywords, except `lambda`;
  - No `'` and `"`;
  - No numbers, except `0`.

> I don't why, but the code doesn't work correctly...

### How to use
```py
from pyfuck import brainfuck

code = """
++++++++++[>++++++++>+++++++++++>++
++++++++>++++>+++>++++++++>++++++++
++++>+++++++++++>++++++++++>+++++++
++++>+++>+<<<<<<<<<<<<-]>-.>--.>---
.>++++.>++.>---.>---.>.>.>+.>+++.>.
"""
code = brainfuck(code)
code.exec()  # Ola, Mundo!
```
```py
code.a == [0, 79, 108, 97, 44, 32, 77, 117, 110, 100, 111, 33, 10, 0, ...]
```
