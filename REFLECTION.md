# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**

 I gained knowledge about how threads mimic CPU scheduling and run concurrently. My output uses a fixed time quantum (4000 ms) to execute several processes (P1–P11) in a round robin fashion. After receiving CPU time, each thread yields and, if unfinished, returns to the ready queue.

Additionally, I comprehended thread states like completed, waiting, and running. P7 and P10, for instance, completed their execution earlier than P2 and P3, which needed many cycles. I now have a better understanding of how multithreading increases CPU consumption

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**

Managing the scheduling mechanism and properly handling context switching was the most difficult aspect. In particular, making sure that every process maintains its remaining burst time after its quantum and returns to the ready queue.

Debugging was made more difficult by thread handling problems I encountered, like a ClassCastException and improper queue behavior.

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

By methodically debugging and closely examining the results, I was able to resolve these problems. For instance, I tracked process behavior using the printed logs (such as "added to ready queue" and "remaining time").

Additionally, I enhanced queue handling and corrected mistakes like wrong casting. It was possible to verify that all procedures were carried out correctly and successfully by running the application several times.

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

In practical applications, multithreading is frequently utilized. Web browsers, for instance, use several threads to load pages, play videos, and process user input all at once.

The scheduler in this assignment mimics the effective management of several processes by an operating system. Similar to this, threads are used in mobile apps and games to guarantee fluid performance without freezing.

---

## Additional Reflections (Optional)

### What would you like to learn more about?

I'm interested in learning more about sophisticated scheduling algorithms like Multilevel Queue Scheduling and Priority Scheduling, as well as how thread synchronization functions.

---

### How confident do you feel about multithreading concepts now?

Intermediate

I am familiar with the fundamentals of scheduling, context switching, and thread execution. I still need to practice sophisticated thread interactions and synchronization, though.

---

### Feedback on the assignment

Understanding how CPU scheduling functions in practice was greatly aided by the assignment. The output's ready queue, quantum execution, and statistics visualizations make the ideas simpler to comprehend. Debugging multithreading problems, however, was difficult and needed close attention.
