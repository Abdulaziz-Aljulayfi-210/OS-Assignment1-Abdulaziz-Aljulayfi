# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

A process is a complete program with its own independent memory, separate from other programs. A thread, on the other hand, is a small part of a process that shares the same memory and resources with other threads. We used threads in this assignment because they are lighter on the system, faster to execute, and share data between them is much easier than creating separate processes. If you look at the code, all processes P1, P2, and others are within a single map and list, which is because they are threads within a single process.

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

In a Round-Robin system, if a process finishes its quantum run but isn't completed, the scheduler removes it from the processor and returns it to the end of the queue to give subsequent processes a chance. We see this in the output when a message appears saying the process "yields CPU" and then it's added back to the queue "added to ready queue." This ensures that no single process takes too long and keeps other processes waiting indefinitely, thus achieving fairness for all

Example from my output:
```

  ? P1 executing quantum [3000ms]
  ? Quantum progress: [███████████████] 100%
  ? P1 completed quantum 3000ms │ Overall progress: [████████░░░░░░░░░░░░] 43%
     Remaining time: 3835ms
  ? P1 yields CPU for context switch

  ? P1 (Priority: 1) added to ready queue │ Burst time: 6835ms
```

**Explanation of example:**
[Explain what's happening in the output snippet you pasted]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**



1. **New**: This is the first stage of P1 and it happens when the program creates a Thread Object in the code using the statement Thread thread = new Thread(process) but before the scheduler actually starts running it.

2. **Runnable**: P1 moves to this state as soon as the scheduler calls the thread.start() method. Here the process is ready and waiting its turn in the Ready Queue for the processor to pick it up.

3. **Running**: Here, P1 is receiving the processor and executing its code. We know this when the message "P1 executing quantum" appears on the screen and the progress bar starts moving.

4. **Waiting**: P1 enters a waiting state when the program calls Thread.sleep() to simulate the execution time of the operation, or when the scheduler makes the main thread wait for its slice to finish using the join() method.

5. **Terminated**:This is the last state, and it is reached by P1 when its Burst Time is completely finished and becomes zero, and the screen prints the message "P1 finished execution" and so its thread stops and ends completely.

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

Example 1: Web Servers

Description: Imagine a website like Amazon or Twitter where thousands of people visit simultaneously, each requesting a specific page. The server creates a separate thread for each request to serve everyone.

Why Round-Robin works well here: The Round-Robin system is excellent because it distributes processing time equally across all requests. This prevents users from waiting too long because another user is downloading a large file. This provides fast responsiveness for everyone, making the website feel seamless for all users.

Example 2: Multimedia Players

Description: When you play a YouTube video or a movie on your device, the player needs to perform many tasks simultaneously, such as audio processing, reading video data, and updating the timeline (seek bar).

Why Round-Robin works well here: Round-Robin ensures that all these tasks are performed in a regular and very fast manner, so the audio doesn't precede the video, and the program doesn't freeze if you try to touch the screen. This provides predictability in the program's performance and makes for a smooth, uninterrupted viewing experience.

---

## Summary

**Key concepts I understood through these questions:**
1. 
2. 
3. 

**Concepts I need to study more:**
1. 
2. 
