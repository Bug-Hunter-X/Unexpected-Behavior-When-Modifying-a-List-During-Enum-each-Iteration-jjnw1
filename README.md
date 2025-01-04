# Elixir List Modification During Enum.each Iteration

This example demonstrates an issue that can arise when attempting to modify a list while iterating over it using `Enum.each` in Elixir.  Since lists in Elixir are immutable, directly modifying the list within the `Enum.each` callback doesn't affect the original list.

The `bug.ex` file shows the original code with the issue, resulting in the list not being modified as intended. The `bugSolution.ex` shows a corrected solution that utilizes `Enum.filter` to achieve the desired result.