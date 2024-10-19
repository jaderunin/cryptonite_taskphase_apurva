## change ownership 
Since the permission of flag file is with the root, simply catting the file as hacker user won't work. Thus, changed its group from root to hacker and read the file.
Here, you can see that the flag is owned by the root user (the first root in that line) and the root group (the second root in that line). When we try to read it as the hacker user, we are denied. However, if we were root (a hacker's dream!), we would have no problem reading this file:
> flag: <img width="794" alt="Screenshot 2024-10-19 at 11 27 40 PM" src="https://github.com/user-attachments/assets/afe661ec-ba8d-4cb8-98f5-97587cf8c974">
## groups and files 
group ownership can be changed with the chgrp (change group) command! Unless you have write access to the file and membership in the new group, this typically requires root access
> flag: 
<img width="530" alt="Screenshot 2024-10-19 at 11 29 25 PM" src="https://github.com/user-attachments/assets/42561319-3d59-4b3e-bc75-09a8a8f5c455">
<img width="556" alt="Screenshot 2024-10-19 at 11 29 29 PM" src="https://github.com/user-attachments/assets/765eefa0-0671-4401-8b01-4d3162dafb6b">
## group names 
There is a convention in Linux that every user has their own group, but this does not have to be the case
## executable files 
we need to add this permission to the hacker user
> flag: hacker@permissions~executable-files:/$ chmod u+x /challenge/run
> hacker@permissions~executable-files:/$ /challenge/run
## tweaking practice 
didnt get it, still trying
## setting practice
non-root users need elevated access to do certain system tasks. The system admin can't be there to give them the password every time a user wanted to do a task that only root/sudoers can do. The "Set User ID" (SUID) permissions bit allows the user to run a program as the owner of that program's file.
<img width="685" alt="Screenshot 2024-10-19 at 11 35 34 PM" src="https://github.com/user-attachments/assets/beb2b385-0143-4ea2-bb52-84d35c63ee2e">
then we run cat/flag to get flag
