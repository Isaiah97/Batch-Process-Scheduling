# Batch-Process-Scheduling
This is assignment 2 of COMP322.

-------------------------------------------------------------------

COMP 322/L—Introduction to Operating Systems and System Architecture
Assignment #2—Batch Process Scheduling

Objective:
To calculate the timing parameters of batch processes based on different scheduling algorithms.

Specification:
The program mimics the execution of different processes under different scheduling algorithms.
The simulation maintains a table that reflects the current state of the system, based on choosing
from a menu of choices, where each choice calls the appropriate procedure, where the choices
are:

1) Enter parameters
2) Schedule processes with FIFO algorithm
3) Schedule processes with SJF algorithm
4) Schedule processes with SRT algorithm
5) Quit program and free memory

Assignment:
• Create a table to record the status of different processes based on the following parameters:
o id: the unique identifier of the process [auto-generated, starting from 1—do not
input from the user]
o arrival: the point in time when the process enters the ready list to be executed by the
CPU [input from the user]
o total_cpu: the amount of CPU time the process will consume between arrival and
departure [input from the user]
o total_remaining: the amount of CPU time remaining for a process to complete [used
for SRT scheduling only]
o done: a flag that indicates whether the process has been successfully completed (1) or
not (0)
o start_time: the time when the process has begun being executed by the CPU
o already_started: a flag that indicated whether the process has already begun (1) or
not (0) [used for SRT scheduling only]
o end_time: the time when the process has been completed by the CPU
o turnaround_time: the sum of the total CPU time and the waiting time (alternatively:
the difference between the end time and the arrival time)
• Calculate the values for the start_time, end_time, and turnaround_time for each process
based on the selected scheduling algorithm.

What NOT to do:
• Do NOT modify the choice values (1,2,3,4,5) or input characters and then try to convert them to
integers--the test script used for grading your assignment will not work correctly.
• Do NOT turn in an alternate version of the assignment downloaded from the Internet (coursehero,
chegg, reddit, github, ChatGPT, etc.) or submitted from you or another student from a previous
semester—the test cases from this semester will not work on a previous semester’s assignment.
• Do NOT turn in your assignment coded in another programming language (C++, C#, Java).

What to turn in:
• The source code as a C file uploaded to Canvas by the deadline of 11:59pm PST (-20% per
consecutive day for late submissions, up to the 4th day—note 1 minute late counts as a day late, 1
day and 1 minute late counts as 2 days late, etc.)
• As a note, even though your code may compile on a compiler you have installed on your
computer, I do not have access to your computer. I will be using the following free online
compiler for testing, so make sure your code compiles with the following online C compiler
before submitting: https://www.onlinegdb.com/online_c_compiler
If it does not compile with the above compiler, the default grade is 0 points since I cannot run it.

