# Lab Reflection: Git Version Control + Debugging (BuggyProgram)

## Student Name
Zeigler, Austin G.

## GitHub Repository URL
[https://github.com/azeigler97/cmsc115-unit8lab1]

---

# Commit 1: Initial Commit

## What did you include in this commit?
- All starter files provided for the lab, including `BuggyProgram.java` and this `README.md` template[cite: 3].

## What was the purpose of this commit?
- To establish a stable baseline version of the project in Git before making any code modifications or bug fixes.

---

# Commit 2: Task 1 (getGrade)

## Which tests in Task1Test were failing before your fix?
- Boundary tests for scores around 80 and 90, as well as cases where the return strings were mismatched with the expected categories.

## What was the issue in the code?
- The conditional logic checked thresholds incorrectly and swapped the return values for "Exceeds" and "Meets".

## What change did you make to fix it?
- Reordered the conditional statements from highest to lowest score and updated the relational operators to use inclusive thresholds (`>=`).

## How did the tests help guide your fix?
- Running the unit tests immediately pointed out which specific score ranges failed, making it clear which conditional branch was misclassifying the grade.

---

# Commit 3: Task 2 (sumEvenNumbers)

## Which tests in Task2Test were failing before your fix?
- Tests involving arrays with mixed numbers, empty arrays, or negative numbers threw index out-of-bounds exceptions or returned incorrect initial offset sums.

## What was the issue in the code?
- The sum accumulator was incorrectly initialized to `1` instead of `0`, and the loop condition used `<=` instead of `<`, causing an `ArrayIndexOutOfBoundsException` at the end of the array.

## What change did you make to fix it?
- Initialized `sum = 0` and changed the loop condition to `i < values.length`.

## How did the tests help guide your fix?
- The assertion failures showed the exact expected versus actual sums, making it clear when odd numbers or improper initialization values were skewing the results.

---

# Commit 4: Task 3 (sumRange)

## Which tests in Task3Test were failing before your fix?
- Tests checking boundary behaviors or ranges where the start value is greater than the end value (descending ranges).

## What was the issue in the code?
- The original loop only handled ascending sequences and lacked support for inverted bounds.

## What change did you make to fix it?
- Added conditional logic to handle both ascending and descending range loops correctly.

## How did the tests help guide your fix?
- The assertion failures highlighted incorrect totals when boundaries crossed or inverted, directing me straight to the loop conditions.

---

# Overall Reflection

## Which task was the easiest to fix? Why?
-

## Which task was the most difficult? Why?
-

## How did Git help you track your progress through the debugging process?
-

## Why is it important to make small, frequent commits when debugging code?
-

## What did you learn about using JUnit tests to guide debugging?
-

---

# Commit 5: Final Reflection

## What did you complete or update before making this final commit?
-

## Why is it useful to document your work after completing a programming task?
-