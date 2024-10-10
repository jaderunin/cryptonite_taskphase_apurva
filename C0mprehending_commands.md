
#  COMPREHENDING COMMANDS 
Provides an introduction to some useful Linux commands. 
## cat: not the pet, but the command!
Cat is an extremely critical command and is used for reading out files. 
When more than one file is provided in the argument, conCATenaation takes place. 
If no files are provided, then cat will read from the terminal input and output it. 
> flag: Connected!
hacker@commands~cat-not-the-pet-but-the-command:~$ pwd
/home/hacker
hacker@commands~cat-not-the-pet-but-the-command:~$ ls
hacker@commands~cat-not-the-pet-but-the-command:~$ cat flag
pwn.college{chXZ0p39Tz8eHmZoHQYnd3dltGr.dFzN1QDL1YjN0czW}
hacker@commands~cat-not-the-pet-but-the-command:~$ 
## catting absolute paths 
We learn that you can specify the cat command with absolute paths as arguments. 
> flag is found by using cat /flag
## more catting practice 
We learn that you can specify the full path to files when using commands like cat, which allows you to access files located in different directories without changing your current working directory and if you can’t change directories (using cd), you must rely on absolute paths to retrieve files.
> flag is found by finding the path of flag using - find / -name "flag" and then different paths were given i checked the right absolute path then used cat (absolutepath)
## grepping for a needle in a haystack 
Sometimes, files are too big to use cat, hence we use the grep command instead. The grep command is used to search for the contents we need. Grep will search the file for lines of text containing our keyword and print them to the console.
> flag is found using grep pwn.college /challenge/data.txt
## listing files 
ls will list files in all the directories provided to it as arguments, and in the current directory if no arguments are provided.
> flag is found by viewing all files
>  ls /challenge
## touching files 
You can create a new, blank file by touching it with the touch command. 
> flag:
> cd /tmp
> touch pwn
> touch college
> /challenge/run
## removing files 
In Linux, you remove files with the rm command. 
> flag is found by create delete_me file using touch, delete it using rm cmd and then run /challenge/check
> touch delete_me
> rm delete_me
> /challenge/check
## hidden files 
ls doesn't list all the files by default. Linux has a convention where files that start with a . don't show up by default in ls and in a few other contexts. To view them with ls, you need to invoke ls with the -a flag. 
> flag is found by finding the flag file in / , which is starting with '.' thus a hidden file
thus we need to use ls -a to view hidden files
then we will use cat cmd to read the file
> cd /
> ls -a
> cat  .flag-215601236318974
## an epic filesystem quest 
> flag is found by using cat , ls and cd comd repeatedly to find chain of clues leading to flag
## making directories 
You make directories using the mkdir command.
> flag is found by  creating 'pwn' directory in /tmp using mkdir cmd and then create college file in /tmp/pwn using touch cmd
> then run /challenge/run to get flag
> cd /tmp
> mkdir pwn
> cd pwn
>touch college
> /challenge/run
## finding files 
Files are found using the find command. 
The find command takes optional arguments describing the search criteria and the search location. If you don't specify a search criteria, find matches every file. If you don't specify a search location, find uses the current working directory (.).
> flag is found by find / -name flag
>cat /usr/share/doc/libec5/flag
## linking files 
To get two programs to access the same data, we must link the files; but the programs expect that data to be in two different locations. The solution to this is links. 

Links in a filesystem come in two types: hard links and soft links (also known as symbolic links). Here’s an analogy to understand the difference:

	•	Hard Link: Think of this like having multiple addresses for the same apartment (e.g., Apt 2 vs. Unit 2). Each address leads directly to the same place.
	•	Soft Link (Symbolic Link): This is like moving to a new apartment and having the postal service forward your mail from your old address to your new one.

In a filesystem, a file is like an address for the data it contains. A hard link is an alternate address that points directly to the same data. Accessing a hard link or the original file gives you the same content immediately. In contrast, a soft link contains the name of the original file. When you access a symbolic link, Linux recognizes it as a link, looks up the original file name, and accesses that file instead.

Both types of links allow you to reach the original data, but they work differently. Hard links are simpler to explain but come with limitations and issues, which is why symbolic links are more commonly used.

Creating Symbolic Links

You can create a symbolic link using the ln command with the -s option, as shown below:

cat /tmp/myfile
# Output: This is my file!

ln -s /tmp/myfile /home/hacker/ourfile

cat ~/ourfile
# Output: This is my file!

In this example, you can see that accessing the symlink (~/ourfile) gives you the contents of the original file (/tmp/myfile).

Identifying Symlinks

You can identify a symlink in several ways. One method is to use the file command, which tells you what type of file you are dealing with:

file /tmp/myfile
# Output: /tmp/myfile: ASCII text

file ~/ourfile
# Output: /home/hacker/ourfile: symbolic link to /tmp/myfile

This output shows that ~/ourfile is a symbolic link pointing to /tmp/myfile.
> flag is found by: rm not-the-flag
> ln -s ~/flag ~/not-the-flag
> /challenge/catflag

> flag is found by 


