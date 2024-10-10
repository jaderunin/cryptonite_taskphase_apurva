
## matching with *
intro nested arguments 
> flag: find -name file_name
## matching with ?
use ? which is a single char wildcard to change directory to /challenge
replace c and l with ?
> flag: cd /?ha??enge
> ./run
## matching with []
1. change directory to /challenge/files
2. 'file_[bash]' as we need the bracket glob files_b, files_a, files_s,files_h
3. run with /challenge/run
> flag:cd /challenge/files
> /challenge/run files_[bash]>
## matching paths with []
do not change cwd
add the path '/challenge/files' to the argument 'file_[bash]'
> flag: /challenge/run /challenge/files/file_[bash]
## mixing globs
glob files 'challenging','educational'and 'pwning' using <6 char
first char of every file is unique
> flag: cd /challenge/files
> /challenge/run [cep]*
## exclusionary globbing
exclude files starting with 'p','w'and 'n' in /challenge/files using [^] argument
> flag: cd /challenge/files
> /challenge/run [^pwn]*
