# Dart Async Error Handling: Silent Exception Swallowing

This repository demonstrates a common error in Dart asynchronous programming where exceptions are silently swallowed within async functions if the `rethrow` keyword is omitted. The `bug.dart` file shows the problematic code, while `bugSolution.dart` provides the corrected version.

The issue arises when an exception occurs within an `async` function's `try-catch` block. If the exception isn't explicitly re-thrown using `rethrow`, the error is not propagated up the call stack, leading to unexpected behavior and difficulty in debugging.

The corrected code showcases the importance of `rethrow` for proper error handling in asynchronous operations.