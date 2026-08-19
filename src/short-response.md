# Short Response Questions

## Question 1: Promise States

What are the three states of a Promise? For each state, explain what it represents and which Promise method (`.then()` or `.catch()`) is used to handle it.

**Your Answer:**

The three states of a Promise are pending, fulfilled, and rejected. Pending means the Promise is still waiting for the operation to finish. Fulfilled means the operation was successful, and `.then()` is used to handle the successful result. Rejected means the operation failed, and `.catch()` is used to handle the error.

## Question 2: Callback Hell vs. Promise Chaining

Explain why deeply nested callbacks (callback hell) are problematic, and describe how Promise chaining with `.then()` solves this problem.

**Your Answer:**

Callback hell happens when callbacks are nested inside of other callbacks, which makes the code difficult to read, understand, and debug. Promise chaining solves this by using `.then()` to run asynchronous operations one after another without deeply nesting them. This makes the code more organized and easier to follow.

## Question 3: Error Handling with `.catch()`

If you have a chain of three `.then()` calls followed by a single `.catch()`, and the second `.then()` throws an error, what happens? Why is this behavior useful?

**Your Answer:**

If the second `.then()` throws an error, the rest of the `.then()` chain is skipped and the error is passed to the `.catch()`. The `.catch()` handles the error so the program can respond to the problem instead of crashing. This is useful because one `.catch()` can handle errors from multiple steps in the Promise chain.
