# Reflection Questions

## Instructions
Answer the following questions about your learning experience. Each answer should be **at least 5-7 sentences** and show your understanding.

---

## Question 1: What did you learn about multithreading?

**Your Answer:**

I learned that multithreading is a powerful tool that allows a program to perform multiple tasks concurrently, thus improving processor efficiency. I gained a practical understanding of the thread lifecycle, where a process starts in standby mode, then executes, and may return to the queue if it doesn't finish within the time quantum segment. I was impressed by the complexity of the thread coordination; each process in the simulation was an independent thread controlled by a scheduler. I also learned how the join() method helps ensure that a thread finishes executing before the processor moves to the next task, preventing interference.

---

## Question 2: What was the most challenging part of this assignment?

**Your Answer:**

The most challenging part for me was implementing the third feature related to accurately calculating the waiting time for each process. The difficulty lies in the fact that the Round-Robin algorithm makes the process enter and exit the Ready Queue multiple times, requiring a high level of concentration to determine the exact entry and exit times. I had to understand precisely when to start time calculation upon creation or when returning to the queue after the quantum process has finished, and when to stop linking the code concepts with the system's real-time using System.currentTimeMillis. This required significant thought to avoid errors. This challenge is directly related to the concept of context switching and how this switching affects the overall system performance.

---

## Question 3: How did you overcome the challenges you faced?

**Your Answer:**

I overcame these challenges by starting by reviewing the course material to gain a deeper understanding of the scheduling algorithm. I also used artificial intelligence to solve some of the problems I encountered in the code. Breaking down the required features into smaller tasks was also very helpful. I began by adding the priority, then the switch counter, and finally the wait time. After ensuring the integrity of the previous parts, I also researched the Java documentation to understand how the Thread class works and how to manage queues using Queue and Map. Ultimately, trial and error, and manually comparing the program output with the expected results, played a significant role in arriving at the correct solution.

---

## Question 4: How can you apply multithreading concepts in real-world applications?

**Your Answer:**

[Give specific examples from real applications you use (web browsers, games, mobile apps, etc.). Explain why threads are useful in those scenarios. Connect to what you learned in this assignment.]

---

## Additional Reflections (Optional)

### What would you like to learn more about?

[Any topics related to threading, concurrency, or operating systems that you're curious about?]

---

### How confident do you feel about multithreading concepts now?

[Rate yourself and explain: Beginner / Intermediate / Confident]

[Explain your rating - what do you understand well? What needs more practice?]

---

### Feedback on the assignment

[Any comments about the assignment? Was it helpful? Too easy/hard? Suggestions for improvement?]
