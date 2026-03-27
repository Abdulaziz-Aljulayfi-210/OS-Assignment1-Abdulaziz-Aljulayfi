# Development Log

## Instructions
Document your development process as you work on the assignment. Add entries showing:
- What you worked on
- Problems you encountered
- How you solved them
- Time spent

**Requirements**: Minimum 5 entries showing progression over time.

---

## Example Entry Format:

### Entry 1 - [April 1, 2026, 2:30 PM]
**What I did**: Forked the repository and set up my student ID

**Details**: 
- Created GitHub account with university email
- Forked the starter repository
- Changed student ID on line 92 to my actual ID (441234567)
- Compiled and ran the program successfully

**Challenges**: Had to install JDK first because javac wasn't recognized

**Solution**: Downloaded JDK 17 from Oracle website and set PATH variable

**Time spent**: 30 minutes

---

## Your Development Log:

### Entry1 March 21, 2026, 4:00 PM

What I did: Downloaded the repository

Details: I forked the repository and changed the university ID to 445050210

Challenges: I encountered a problem linking GitHub and VS

Solution: I downloaded Git to link them

Time taken: 1 hour

---

### Entry 2 March 22, 2026, 5:00 PM

What I did: Added the Priority feature
Details: I added a priority field to the Process class and modified the constructor to accept a random value between 1 and 5

Challenges: How to ensure the priority is displayed correctly when a process enters the queue

Solution: I modified the `addProcessToQueue` method to include printing the priority value next to the process name

Time taken: 1 hour 

---

### Entry 3 March 22, 2026, 7:00 PM

What I did: Added the second feature, Context Switch Counter.

Details: Defined a static variable, contextSwitchCount, to count the number of times the processor switches between processes.

Challenges: Counting the first process as a context switch.

Solution: Incremented the counter each time a while loop starts to pull a new process from the queue.

Time taken: 1 hour

---

### Entry 4 March 23, 2026, 11:00 PM

What I did: Added the third feature (Waiting Time)

Details: I added variables to track the creation time, the time a process enters the queue, and calculate the total time a process spends waiting its turn.

Challenges: Execution times overlapped with wait times in Run-Robin.

Solution: I used System.currentTimeMillis() to record the moment a process exits the queue and the moment it rejoins it.

Time taken: 3Hours

---

### Entry 5 March 24, 2026, 4:00 PM

What I did: Created the final summary table

Details: Programmed the `displayWaitingTimeSummary` method to display the results

Challenges: Formatted the columns in the table to be equal in length regardless of the number lengths

Solution: Used `String.format` to adjust the spacing

Time taken: 1 hour

---

### Entry 6 - [Optional - Date and Time]
**What I did**: 

**Details**: 

**Challenges**: 

**Solution**: 

**Time spent**: 

---

## Summary

Total time spent: 7 hours

Most challenging part: Accurately calculating the wait time, as processes in Round-Robin enter and exit the queue multiple times before finishing.

Key takeaways: How to use threads to simulate real-world operating system behavior, and how to manage process queues.

What I'll do differently next time: I'll try implementing a Round-Robin development.
