# Lua pairs iterator unexpected behavior with modified tables

This repository demonstrates an uncommon bug in Lua related to the `pairs` iterator and table modification during iteration.

The `bug.lua` file contains a function `foo` that recursively iterates through a table using `pairs`.  If the table is modified within the loop, `pairs` may not visit all elements as expected. This can lead to unexpected results, including skipped elements or even infinite loops.

The `bugSolution.lua` file provides a solution that addresses this issue, demonstrating correct ways to handle table modification within iteration.