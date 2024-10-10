## redirect output
redirect stdout to files. You can accomplish this with the > character
flag: echo PWN > COLLEGE
## redirecting more output:
> flag: /challenge/run > myflag
> cat myflag
## appending output: 
> flag: /challenge/run >> /home/hacker/the-flag
> cat /home/hacker/the-flag
## redirecting errors 
> flag: cat myflag
## redirecting input
> flag: echo COLLEGE > PWN
> /challenge/run < PWN
## grepping stored results
> flag: /challenge/run | grep "pwn.college"
## live output
> flag: /challenge/run | grep "pwn.college"
## errors: 
> flag:/challenge/run 2>&1 | grep "pwn.college"
## piped data with tee
> flag: didnt get :(
## multi step prog
> flag: /challenge/hack | tee >( /challenge/the ) >( /challenge/planet )
## stderr and stdout
> flag: /challenge/hack > >( /challenge/planet ) 2> >( /challenge/the )
