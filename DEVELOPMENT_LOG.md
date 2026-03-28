Development Log - OS Assignment 1

Entry 1 - [March 20, 2026, 4:30 PM]

What I did: GitHub account setup and Forking.
Details:

I created my GitHub account using the university email as required.

I forked the starter repository from the professor's page.

I changed the name of the repository to OS-Assignment1-Azzam-AlFawaz.
Challenges: I didn't know how to change the repository name at first after forking.
Solution: I searched through the "Settings" tab and found the rename option there.
Time spent: 40 minutes

Entry 2 - [March 22, 2026, 7:15 PM]

What I did: Environment setup and setting my Student ID.
Details:

I opened the project folder in VS Code.

I changed the student ID on line 92 to my actual ID (445050167).

I tried to run the code to test if the environment was ready.
Challenges: The terminal was not recognizing "javac" to compile the code.
Solution: I had to install the Java Extension Pack in VS Code and set up the JDK path.
Time spent: 35 minutes

Entry 3 - [March 24, 2026, 3:00 PM]

What I did: Adding Priority (Feature 1).
Details:

I added the priority variable to the Process class.

I updated the constructor so it takes the priority value when creating a process.

I modified the "addProcessToQueue" method to show the priority in the output.
Challenges: The priority was showing 0 for all processes at the beginning.
Solution: I fixed the random code to use "random.nextInt(5) + 1" so it generates numbers between 1 and 5 correctly.
Time spent: 1 hour

Entry 4 - [March 26, 2026, 9:30 PM]

What I did: Context Switch Counter (Feature 2).
Details:

I created a static variable called "contextSwitchCount" to track CPU switches.

I added the code to increment this counter inside the scheduler loop.

I added a final message at the end to show the total count of switches.
Challenges: The counter was showing a very high number that was wrong at first.
Solution: I moved the "contextSwitchCount++" line to the correct place right when a process is polled from the queue.
Time spent: 50 minutes

Entry 5 - [March 28, 2026, 10:15 PM]

What I did: Waiting Time and fixing syntax errors.
Details:

I added the logic to track how long each process stays in the ready queue.

I created the final summary table to show Burst Time and Waiting Time.

I spent a lot of time fixing red errors in the file.
Challenges: I had many errors because I accidentally deleted some closing brackets "}" and missed a ")" while typing the new code, which caused "illegal start of expression" errors.
Solution: I carefully checked the brackets and parentheses one by one until the code compiled and ran successfully.
Time spent: 1.5 hours

Summary

Total time spent on assignment: 4.5 hours.
Most challenging part: Debugging the code and fixing the bracket errors that happened while I was manually typing the new features.
Most interesting learning: Understanding how the Round Robin algorithm actually manages multiple threads and switches between them.
What I would do differently next time: I will try to be more organized while writing the code and double-check my brackets after every new block I add to avoid long debugging sessions.
