##  listing 
ps either stands for "process snapshot" or "process status", and it lists processes.
each process has a numerical identifier (the Process ID, or PID), which is a number that uniquely identifies every running process in a Linux environment.
here are two ways to specify arguments.

"Standard" Syntax: in this syntax, you can use -e to list "every" process and -f for a "full format" output, including arguments. These can be combined into a single argument -ef.

"BSD" Syntax: in this syntax, you can use a to list processes for all users, x to list processes that aren't running in a terminal, and u for a "user-readable" output. These can be combined into a single argument aux.
both display the user (USER column), the PID, the TTY, the start time of the process (STIME/START), the total utilized CPU time (TIME), and the command (CMD/COMMAND). ps -ef additionally outputs the Parent Process ID (PPID), which is the PID of the process that launched the one in question, while ps aux outputs the percentage of total system CPU and Memory that the process is utilizing. 
> flag: ps -ef then run the executable file
## killing
kill will terminate a process in a way that gives it a chance to get its affairs in order before ceasing to exist
