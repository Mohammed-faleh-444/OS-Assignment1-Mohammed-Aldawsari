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

## Entry 1 - [march28,2026,4pm]
**What I did**: started the project and understood the given code

**Details**: i read the assignment instructions and understand how the scheduler work and run the code

**Challenges**: i did not understand how the threads are used in the code at first

**Solution**: i watched a video who make me learn about runnable and threads in java

**Time spent**: 1 - 1:30 hour

---

### Entry 2 - [march29,2026,6am]
**What I did**: modified the student id and tested randomness

**Details**: changed the student id to my actual id and observed how number of processes and time quantum change and tested running the code multiple times

**Challenges**: i was confused why the output changes

**Solution**: understood that random depends on the student id seed

**Time spent**: 30 minutes

---

### Entry 3 - [march29,2026,8am]
**What I did**: worked on process execution logic

**Details**: focused on run() method and understood how time quantum is applied and checked how remaining time decreases

**Challenges**: did not understand how waiting time is calculated

**Solution**: reviewed the formula used System.currentTimeMillis() to track time

**Time spent**: 1 hour

---

### Entry 4 - [march29,2026,7pm]
**What I did**: added waiting time and context switch tracking

**Details**: added totalWaitingTime variable and updated it inside run() method and added contextSwitches counter in main

**Challenges**: witing time values looked incorrect at first

**Solution**: fixed by updating creationTime after each execution

**Time spent**: 1 hour

---

### Entry 5 - [march29,2026,8pm]
**What I did**: improved output and added summary

**Details**: added colored output using ANSI codes and added summary table at the end and printed burst time and waiting time for each process

**Challenges**: had problem formatting the output table

**Solution**: used "\t" for spacing between columns

**Time spent**: 45 minutes

---

### Entry 6 - [march30,2026,4pm]
**What I did**: final testing and debugging

**Details**: ran the program multiple times and checked if all processes finish correctly and verified waiting time and context switches

**Challenges**: small syntax error in print statement

**Solution**: fixed quotation and spacing issue

**Time spent**: 30 minutes

---

## Summary

**Total time spent on assignment**: [4 hours 25 minutes]

**Most challenging part**: understanding how waiting time is calculated using system time

**Most interesting learning**: using threads and simulating CPU scheduling was interesting

**What I would do differently next time**: i would start earlier and try to use priority in scheduling instead of just storing it
