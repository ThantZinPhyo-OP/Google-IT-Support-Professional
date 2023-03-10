# Operating System and You: Becoming a Power User | Week - 5

## Process Utilization

### Question 1

Which of the following PowerShell commands will tell you which process on your system is using the most CPU resources?

Get-Process | Sort CPU -descending | Select -first 1 -Property ID,ProcessName,CPU  ( Correct )

Get-Process | Sort RAM -descending | Select -first 1 -Property ID,ProcessName,CPU 

cpu_usage.exe | top -1

Answer - Wohoo! That command will do the trick. It will filter the output of the Get-Process commandlet to determine the top user of the CPU resource, and give its Process ID, name, and the amount of CPU used.


### Question 2

If you have a slow computer, what are some possible culprits that could be causing this? Select all that apply.

High CPU usage ( Correct )

Lots of I/O activity ( Correct )

High RAM usage ( Correct )

Too many processes running ( Correct )

Answer - You nailed it! A slow computer could be a sign of lots of things, but it's always smart to first check the utilization of your resources.


### Question 3

In a Linux machine, what command can you use to safely terminate a process with a PID of 342?

kill 342 ( Correct )

kill -KILL 342

kill -TSTP 342

kill -CONT 342

Answer - Great work! To terminate a process safely, send the SIGTERM signal.


### Question 4

In a Linux machine, what command can you use to absolutely kill a process with a PID of 342?

kill 342

kill -KILL 342 ( Correct )

kill -TSTP 342

kill -CONT 342

Answer - You got it! To kill a process, you'd use the SIGKILL signal.


### Question 5

In a Linux machine, what command can you use to suspend a process with a PID of 342?

kill 342 

kill -KILL 342

kill -TSTP 342 ( Correct )

kill -CONT 342

Answer - Great work! To stop or suspend a running process, you'd send the SIGTSTP signal.