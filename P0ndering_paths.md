
# PONDERING PATHS 
The linux filesystem can metaphorically be referred to as a tree as it contains roots (written as '/'). The root is a directory, that can contain other directories and files. These can be referrenced using their individual 'paths'. Every piece of the path is demarcated with another '/'. 
## The Root 
The style of path, one that starts with the root directory, is referred to as an "absolute path". 
> Invoking "/pwn" gives us the flag 
## Program and Absolute Paths 
Challenges in pwn.college are typically located in the /challenge directory, which is situated directly in the root directory (/). Therefore, the full path to the challenge program is /challenge/run. 
> To execute the program and find the flag we use the command /challenge/run.
## Position thy self 
Here we learn that we can navigate around directories using the 'cd' (change directory) command and passinf a path to it as an argument. We also see that this changes our current working directory. 
"~" shows the current directory that the shell is located at. 
> flag is found by going to the /usr/share/doc/fontconfig directory then running /challenge/run.
## Position Elsewhere 
> flag is found by going to the /proc/67 directory then running /challenge/run.
## Position Yet Elsewhere 
> flag is found by going to the /var/log directory then running /challenge/run.
## implicit relative paths, from /
if you put in absolute paths everywhere, then it really doesn't matter what directory you are in.
A relative path is any path that does not start at root (i.e., it does not start with /).
A relative path is interpreted relative to your current working directory (cwd).
Your cwd is the directory that your prompt is currently located at.
> flag: challenge/run is a relative path, invoked from the right directory!
## explicit relative paths, from /
In most operating systems, including Linux, every directory has two implicit entries that you can reference in paths: . and ... The first, ., refers right to the same directory.
> flag: cd / then ./challenge/run
## implicit relative path
> flag: ./run is a relative path, invoked from the right directory (cd /challenge)
## home sweet home 
> flag: we execute /challenge/run ~/f
> which gives us:
> Writing the file to /home/hacker/f!
> ... and reading it back to you:
