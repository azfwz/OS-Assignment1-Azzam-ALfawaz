Assignment Questions - OS Concepts

Question 1: Thread vs Process

A process is like a big program that has its own memory and resources from the computer. A thread is a smaller part that lives inside a process and shares the same memory. It is much faster and cheaper for the computer to create threads than to create separate processes. In this assignment, we used threads because our simulation is one single program that needs to run tasks together. If we used processes, it would be very slow and use too much memory. Threads are perfect for this because they can easily talk to each other in our Java code.

Question 2: Ready Queue Behavior

In Round-Robin scheduling, if a process doesn't finish its work during the time quantum, it must leave the CPU. The process goes back to the end of the ready queue to wait for its next turn. This ensures that no single process takes all the CPU time and everyone gets a fair chance. You can see this in my program output when a process says "yields CPU for context switch." It is like people waiting in a circle; if your time is up, you go to the back of the line.

Example from my output:

  ⏸ P1 completed quantum 2000ms │ Overall progress: [████░░░░] 50%
     Remaining time: 2000ms
  ↻ P1 yields CPU for context switch
  ➕ P1 added to ready queue │ Burst time: 4000ms


Explanation of example:
In this snippet, P1 finished its 2000ms time quantum but it still has 2000ms of work left. Because it is not finished, the program moves it from the CPU back to the end of the "ready queue." Now, P1 has to wait for other processes like P2 or P3 to finish their turns before it can run again.

Question 3: Thread States

In my simulation, every process like P1 goes through different steps or "states."

New: This is when the code first creates the process object new Process("P1", ...) but the thread hasn't started yet.

Runnable: P1 enters this state when it is added to the processQueue and is waiting for its turn.

Running: P1 is in this state when the CPU picks it and the run() method starts executing the quantum.

Waiting: P1 enters a waiting state when it calls Thread.sleep() to simulate working or when the main thread waits using join().

Terminated: This is the final state when P1 has 0 remaining time and the thread finishes its execution completely.

Question 4: Real-World Applications

Example 1: Web Servers
Description: A web server handles many people trying to visit a website at the same time.
Why Round-Robin works well here: It gives every user a small amount of time so that everyone feels the website is responding. If one person is downloading a huge file, it won't stop other people from seeing the page. This makes the service fair and fast for everyone.

Example 2: Simple Task Managers
Description: Our computers run many small background apps like the clock, anti-virus, and messengers.
Why Round-Robin works well here: It allows the operating system to switch between these apps very quickly. Even if we have many apps open, they all stay updated because each one gets a little bit of CPU time. It keeps the computer smooth and prevents any small app from freezing.

Summary

Key concepts I understood through these questions:

The difference between a process and a thread.

How the Round-Robin algorithm shares time fairly.

The lifecycle of a thread from start to finish.

Concepts I need to study more:

How threads share memory without crashing.

Different types of scheduling algorithms other than Round-Robin.
