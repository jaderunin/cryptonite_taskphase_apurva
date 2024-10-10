
## Learning from documentation 
The typical need you'll have for documentation is just to figure out how to use all programs, and a specific case of that is figuring out what arguments to specify on the command line.
The correct usage of programs depends, in a large part, in the proper specification of arguments to them. Recall the -a of ls -a in the hidden files challenge of the Basic Commands module: that -a was an argument that told ls to list out hidden files as well as non-hidden files. Because we wanted to list out hidden files, invoking ls with the -a argument was the correct way to use it in our scenario.
> flag: /challenge/challenge --giveflag
## Learning complex usage
> flag: /challenge/challenge --printfile /flag
## reading manuals
You can scroll around the manpage with your arrow keys and PgUp/PgDn. When you're done reading the manpage, you can hit q to quit.
The arguments to the man command aren't file paths, but just the names of the entries themselves
> flag: the manual says to use --gfkqag 485 argument to get flag
> man challenge
> /challenge/challenge --gfkqag 485
## Searching Manuals
search the manual for the right argument which gives flag using '/'
> flag:/challenge/challenge  --btlyi
## Searching for Manuals
1. read and understand manual of manual cmd itself
2. find a way to find the challenge manual
3. must use '-k' argument and search 'challenge'
4. read the manual of challenge progrma to get the argument for flag
>  flag: man man
> man -k challenge
> man gwjoazyyda
> /challenge/challenge  --gwjoaz 401
## Helpful Programs
Here, use --help cmd for /challenge/challenge program to learn how to get the flag.
> flag: /challenge/challenge --help
> /challenge/challenge -p
> /challenge/challenge -g 64
## Help for Builtins
here, use help cmd to find argumnets of builtin cmd challenge which gives the flag
> flag: help challenge
> challenge --secret 8Ws6YXFR
