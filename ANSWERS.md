# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A thread is a smaller unit of execution, but a process is a separate program with its own memory and resources.

Threads are faster and lighter than processes, which are heavier and require more time to construct and switch between.

Since the objective of this assignment is to effectively replicate CPU scheduling, threads were used. The simulation is more realistic and effective when threads are used because they enable quicker context switching and shared access to the ready queue.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

A process in Round-Robin scheduling is returned to the ready queue to wait for its next turn if it does not complete within its time quantum.

Example from my output:
```
P2 executed for 4000ms, remaining time: 3000ms
P2 added to ready queue

```

**Explanation of example:**

In this example, process P2 did not finish its burst time during its quantum (4000ms), so it was paused and placed back in the ready queue. It will run again later when its turn comes, ensuring fairness among all processes.

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

1. **New**: [P1 is in the New state when it is created using the Thread constructor but has not started yet.]

2. **Runnable**: [P1 becomes Runnable after calling start(), where it is ready to be scheduled by the CPU]

3. **Running**: [P1 is in the Running state when it is actively executing during its time quantum (e.g., executing for 4000ms).]

4. **Waiting**: [P1 enters Waiting when it is paused (e.g., during sleep() or waiting for its next turn after being re-added to the queue).]

5. **Terminated**: [P1 reaches Terminated when it finishes its execution completely (remaining time = 0).]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Browser]

**Description**: 

Web browsers handle multiple tasks such as loading pages, running scripts, and playing videos simultaneously.

**Why Round-Robin works well here**: 

Round-Robin ensures fairness between tasks, so no single task blocks the browser. Each task gets CPU time, improving responsiveness.

### Example 2: [Operating System Task Scheduling]

**Description**: 

Operating systems manage multiple processes like background apps, system tasks, and user programs.

**Why Round-Robin works well here**: 

It ensures that all processes get CPU time fairly, preventing starvation and maintaining system stability.

---

## Summary

**Key concepts I understood through these questions:**
1. Difference between threads and processes.
2. Round-Robin scheduling and ready queue behavior.
3. Thread lifecycle and states.

**Concepts I need to study more:**
1. Thread synchronization and race conditions.
2. Advanced scheduling algorithms.
