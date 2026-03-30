# Assignment Questions

## Instructions
Answer all 4 questions with detailed explanations. Each answer should be **3-5 sentences minimum** and demonstrate your understanding of the concepts.

---

## Question 1: Thread vs Process

**Question**: Explain the difference between a **thread** and a **process**. Why did we use threads in this assignment instead of creating separate processes?

**Your Answer:**

[a program that is running and uses its memory and resources is called a process a thread is a part of a process
threads use the memory and resources as the process they belong to
processes are separate from one another
creating a process needs time and resources than creating a thread
in our assignment we used threads because they are easy to manage and fast
threads are also good for simulating CPU scheduling
this is because we need tasks to run in a similar setup and share data with each other easily
threads help us do this]

---

## Question 2: Ready Queue Behavior

**Question**: In Round-Robin scheduling, what happens when a process doesn't finish within its time quantum? Explain using an example from your program output.

**Your Answer:**

[in Round-Robin scheduling if a process does not finish within its time limit it goes back to the queue
this means it waits for its turn again after other processes execute
the process keeps repeating this until its remaining time's zero
this makes sure every process gets a chance to run
Round-Robin scheduling is fair because every process gets a chance to execute]

Example from my output:
```
[P3 executing quantum [2000ms]  
P3 completed quantum 2000ms │ Remaining time: 1500ms  
P3 yields CPU for context switch  
P3 added to ready queue]
```

**Explanation of example:**
[the process P3 did not finish on time
 it still has some time left when it is done with its turn it lets go of the CPU
goes back to the ready queue the process P3 will be chosen again later it will keep running until the process P3 is finished]

---

## Question 3: Thread States

**Question**: A thread can be in different states: **New**, **Runnable**, **Running**, **Waiting**, **Terminated**. Walk through these states for one process (P1) from your simulation.

**Your Answer:**

[Write your answer here. For each state, explain when P1 enters that state during the simulation. Use your understanding of the code to trace through the lifecycle.]

1. **New**: [P1 is in the New state when the thread is created using new Thread(process) but before calling start()]

2. **Runnable**: [P1 becomes Runnable after calling start(), and it is ready to be executed by the CPU]

3. **Running**: [P1 is in the Running state when the CPU executes the run() method for its time quantum]

4. **Waiting**: [P1 enters waiting state when the main thread calls join() to wait for it to finish or when it is waiting for its next turn in the queue]

5. **Terminated**: [P1 becomes Terminated when it finishes all its remaining time and completes execution]

---

## Question 4: Real-World Applications

**Question**: Give **TWO** real-world examples where Round-Robin scheduling with threads would be useful. Explain why this scheduling algorithm works well for those scenarios.

**Your Answer:**

### Example 1: [Web Browser Tabs]

**Description**: 
[when we use a web browser it can have many tabs open at the time each of these tabs in the web browser does its thing 
for example a tab in the web browser can load a page run some scripts the web browser lets all these tabs work together which is really useful]

**Why Round-Robin works well here**: 
[Round-Robin scheduling is really good because it makes sure each tab gets an amount of CPU time
this means the browser will stay responsive it also stops one tab from using up all the resources 
Round-Robin scheduling is important for the browser to work properly each tab will get a turn to use the CPU time so the browser will not get stuck on one tab
this way Round-Robin scheduling helps the browser to keep working]

### Example 2: [Name of application/scenario]

**Description**: 
[An operating system runs many programs at the same time such as background apps and user applications]

**Why Round-Robin works well here**: 
[the Round-Robin method is really good at sharing CPU time between processes this means that each process gets a turn
the Round-Robin system makes sure that everything runs smoothly and quickly it does this by not letting one process take up all the time which's very important
this way the Round-Robin system helps to prevent one process from stopping others for long]

---

## Summary

**Key concepts I understood through these questions:**
1. the difference between threads and processes
2. how Round-Robin scheduling works
3. thread lifecycle and states

**Concepts I need to study more:**
1. advanced scheduling algorithms like priority scheduling
2. thread synchronization and avoiding race conditions
