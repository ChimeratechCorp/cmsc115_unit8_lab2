# Reflection – AI Number Program Lab

##  Student Name:
Robert Cruz

##  GitHub Repository Link:
https://github.com/ChimeratechCorp/cmsc115_unit8_lab2.git

## Iteration 1

What the AI code does:
- From the prompt AI generated some code. Created a method `findResult()` that loops through every number in the
  array, adds each one to a running total, and returns the sum.

Tests passed/failed:
- testBasicArray() failed. Expected 9, but the method returned 26 which was the sum of the array.
- testNegativeNumbers() failed. Expected -1, but the method returned -64.
  Adding negative numbers together makes the result more negative instead
  of finding the largest (closest to zero) value.
- testSingleValue() passed. With only one number in the values array, the sum is the same number, so the wrong logic 
  happened to give the right answer.
- testEmptyArray() failed. Expected -2147483648 Actual 0, the method 
  returned 0 because the loop never runs and the starting total of 0 is returned.

What surprised you:
- From the prompt, I didn't specify what the method was supposed to do. AI generated a method to sum the 
  items in an array Which was pretty cool. The code had no errors, but because I didn't specify the prompt on what the 
  method was supposed to do it didn't pass the logic. It did pass one test through, which was very surprising. 
  It passed by coincidence which means that just because the code passed doesn't mean the code is correct or the logic
  is doing what you want it to do.


Commit message:
- AI-generated implementation

---

## Iteration 2

What changed:
-

What improved:
-

What still failed and why:
-

Commit message:
-

---

## Iteration 3

Final behavior:
-

What was fixed:
-

What you learned:
-

Commit message:
-

---

## Final Reflection

- How did AI responses change across prompts?
- How did testing affect your changes?
- What did version control help you understand?