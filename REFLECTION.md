Reflection Report - MultiThreading Assignment

Question 1: What did you learn about multithreading?

In this assignment, I learned that multithreading is a powerful way to make programs perform multiple tasks at the same time. I specifically practiced how to use the Runnable interface and the Thread class to create and manage processes in Java. It was very interesting to see the different states of a thread, such as when it starts, runs for its quantum, and then yields the CPU. I learned how the Thread.sleep() method can simulate execution time and how Thread.join() is used to wait for a thread to finish. Understanding how context switching happens between threads was a big eye-opener for me regarding how operating systems work. Overall, I now have a much better understanding of how concurrent execution is managed in a professional way.

Question 2: What was the most challenging part of this assignment?

The most challenging part of this assignment for me was managing the code structure while adding the three new features. Specifically, adding the waiting time tracking and the context switch counter required making changes in several places in the code at once. Because the code was getting longer and more complex, I accidentally messed up the brackets { } and parentheses ( ), which caused many red errors in VS Code. It was difficult to trace where the missing brackets were while also trying to keep the Round-Robin logic working correctly. This taught me that multithreaded programs need very careful organization and precise typing to avoid breaking the system. It was a real test of my attention to detail and my ability to read long error logs.

Question 3: How did you overcome the challenges you faced?

I overcame these challenges by taking a very systematic and patient approach to debugging. When I saw the syntax errors in the terminal, I didn't panic, but instead, I started checking the code line by line to find the missing brackets. I used the error messages in VS Code as a guide to pinpoint exactly where the code was failing. I also referred back to the assignment PDF many times to make sure my logic for the priority and waiting time features followed the requirements. Testing the program after every small modification was a strategy that helped me ensure that one feature worked before moving to the next. Finally, re-reading the starter code helped me understand how to integrate my new variables without affecting the existing thread lifecycle.

Question 4: How can you apply multithreading concepts in real-world applications?

Multithreading concepts are used everywhere in the real-world applications we use daily, like web browsers and video games. For example, in a browser, each tab can run on a separate thread so that one heavy website doesn't make the entire browser freeze. In modern video games, different threads are used to handle physics, graphics, and background music simultaneously to keep the gameplay smooth. The Round-Robin scheduling I learned is also applied in servers that handle many users at once to ensure that everyone gets a fair amount of service time. These concepts are also essential for mobile apps that need to download data in the background while the user continues to interact with the screen. Learning these skills helps me understand how to build software that is responsive, fast, and efficient for the users.
