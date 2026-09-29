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
- The method no longer adds up the numbers. It now finds the largest
  value in the array. Its starts by initialing `max` to the first index in array
  then assigns `max` when a new large number is found.
  

What improved:
- 3 of 4 tests passed from the first iteration
- `testBasicArray()` passed returning 9 as expected.
- `testNegativeNumbers()` now passed returning -1. Comparing values instead of
  adding them correctly handles negative numbers.
- `testSingleValue()` passed again but compared for the first
  iteration, the method actually finds the largest value instead of passing by coincidence.


What still failed and why:
- `testEmpyArrary()` failed. Index 0 out of bounds for length 0.
  An empty array has no `[0]` element. My prompt didn't mention testing for empty array, so it didn't make it.
  handle that case.

Commit message:
- Iteration 2: largest value implementation

---

## Iteration 3

Final behavior:
- The findResult method returns the largest integer in the array. If the
  array is empty, it returns Integer.MIN_VALUE (-2147483648). 
- All 4 tests passed.

What was fixed:
- In Iteration two, testEmptyArray crashed because an empty array can't have a `[0]` value.
- To fix the testEmptyArray AI added if statement at the top of the method that checks whether
  values.length is 0 or empty. If it is, the method returns Integer.MIN_VALUE.
- All other fixes were logic based on the prompt that was given to AI.

What you learned:
- AI generation is all based on the prompt given. If you want a specific task complete, 
  you AI prompt to be detailed enough to describe the task you want to be complete. 
- So, the more specific my prompt was the better the AI's code matched what I wanted.
- AI generated code can easily miss edge cases because it only completing code that is specifically asked for. 
  AI didn't consider edge cases until I asked for it directly.

Commit message:
- Complete the Final Reflection section

---

## Final Reflection

- How did AI responses change across prompts?
- AI generated code that I asked for specifically. The code got better the more 
  detailed prompt I gave it. 

- How did testing affect your changes?
- The testing showed the expected results and my actual results and all the methods used for the program
  so I can get an idea what the goal of the application will be. 

- What did version control help you understand?
- Commiting after each iteration gave me record on how the code changed each time. I can use GitHub commit history
  to see previous changes and revert to those changes if I need to. I also learned from last lab to correctly comment 
  each commit to help navigate through commits. 