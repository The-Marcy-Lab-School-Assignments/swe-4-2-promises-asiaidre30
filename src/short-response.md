# Short Response Questions

## Question 1: Promise States

What are the three states of a Promise? For each state, explain what it represents and which Promise method (`.then()` or `.catch()`) is used to handle it.

**Your Answer:** the three states of a `Promise` are `pending`, `resolved` and `rejected`. The `pending` state means that the fetch operation is still going on. The `resolved` state means that the function was a success we got the value we wanted. The `rejected` state means that the function failed we got an error back.To handle promises we use `.then()` because it schedules a callback to be executed when the promise resolves.

## Question 2: Callback Hell vs. Promise Chaining

Explain why deeply nested callbacks (callback hell) are problematic, and describe how Promise chaining with `.then()` solves this problem because it helps the code run cleaner and each async step runs in order, and the errors

**Your Answer:**

deeply nested callbacks (callback hell) are problematic because they make the code messy and its overlaping and hard to read, which is very unorganized. Promise chaining with `.then()` solves this problem

## Question 3: Error Handling with `.catch()`

If you have a chain of three `.then()` calls followed by a single `.catch()`, and the second `.then()` throws an error, what happens? Why is this behavior useful?

**Your Answer:**
If the second `.then()` throws an error, the chain stops and goes straight to the `.catch()`.
This is useful because it **catches** all errors in one
