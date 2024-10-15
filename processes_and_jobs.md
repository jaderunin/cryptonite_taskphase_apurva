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
> flag: 
<img width="709" alt="Screenshot 2024-10-15 at 1 32 12 PM" src="https://github.com/user-attachments/assets/fff3880a-a1f0-402a-8e7a-ffba869ae60c">
## interrupting
cntrl c interrupts the process 
> flag: <img width="691" alt="Screenshot 2024-10-15 at 1 34 09 PM" src="https://github.com/user-attachments/assets/5a316b8a-6f25-49c7-922d-b60ec0290f4b">
## suspending 
You can suspend processes to the background with Ctrl-Z. 
> flag: 
<img width="599" alt="Screenshot 2024-10-15 at 3 24 29 PM" src="https://github.com/user-attachments/assets/16985099-b53d-4787-b86e-da5577cad9da">
## resuming
fg (foreground) resumes the process
> flag: <img width="656" alt="Screenshot 2024-10-15 at 3 25 40 PM" src="https://github.com/user-attachments/assets/26a2da3b-1fa6-40a7-9500-a759dbacad83">
## backgrounding
bg command allows the process to keep running, while giving you your shell back to invoke more commands in the meantime.
>flag: <img width="639" alt="Screenshot 2024-10-15 at 3 27 36 PM" src="https://github.com/user-attachments/assets/4e8e175e-b9cb-4812-a7d4-4a853157c1db">
## foregrounding
here we learn how to fg a bg process 
> flag: <img width="748" alt="Screenshot 2024-10-15 at 3 29 01 PM" src="https://github.com/user-attachments/assets/4d8f1f1d-e3df-491e-b441-15bb8bd5a784">
## starting bg
all you have to do is append a & to the command to start bg process without suspending
> flag: 
<img width="755" alt="Screenshot 2024-10-15 at 3 31 08 PM" src="https://github.com/user-attachments/assets/e7a5287a-fcb6-4d0a-a322-f114347618d6">
## exit codes



