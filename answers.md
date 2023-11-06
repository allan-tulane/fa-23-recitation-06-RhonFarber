# CMPS 2200 Recitation 06
## Answers

**Name:** Rhon Farber
**Name:**_________________________


Place all written answers from `recitation-07.md` here for easier grading.



- **2)**
Recurrence for Work: W(n) = W(n−1) + W(n−2) + O(1)
There is no parallelizability so the work is W(n) = O(2^n)
- **3)**
Recurrence for Span: S(n) = S(n-1) + O(1)
Span: S(n) = O(n)
- **4)**
After inspecting the counts list, an interesting pattern that's emerged is that the amount of calls is equal to the fibonacci sequence, for example:
fib(0) = 1 call
fib(1) = 1 call
fib(2) = 2 calls
fib(3) = 3 calls
fib(4) = 5 calls
So to calculate any fib_recursive(n), it will make calls to fib_recursive(n-1) and fib_recursive(n-2).
- **6)**
The maximum number of times fib_top_down(i) will be called for any particular i is exactly once. This is because the first time fib_top_down(i) is called, it computes the result and stores it in fibs[i]. Later calls for the same i will return immediately after checking fibs[i]. Based on this, the work would be O(n) and the span would also be O(n).
- **8)**
Fi will be read twice for each value of i. The work is O(n) and the span is also O(n). 