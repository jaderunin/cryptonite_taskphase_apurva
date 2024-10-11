# shell variables 
## Printing variables 
echo just prints the stuff we input, while echo $(variable) prints variable data. 
> flag: <img width="508" alt="Screenshot 2024-10-11 at 10 46 52 AM" src="https://github.com/user-attachments/assets/b2bd568c-a27d-4aa3-a4c3-1f1b591ee22b">
## setting variables
While assigning a value to a variable, don't put a spcae between the var name, =, and the value or it tries to run VAR command (DNE). 
Note that this uses VAR and not $VAR: the $ is only prepended to access variables. In shell terms, this prepending of $ triggers what is called variable expansion, and is, surprisingly, the source of many potential vulnerabilities.
> flag: <img width="489" alt="Screenshot 2024-10-11 at 10 56 26 AM" src="https://github.com/user-attachments/assets/d504271e-dd37-4a63-a172-f2ff604e6d3c">
## Multi word variables 
multi word variables need to be put in quotes as we can't have spaces, as discussed above. 
> flag: <img width="498" alt="Screenshot 2024-10-11 at 11 07 58 AM" src="https://github.com/user-attachments/assets/e038b15c-5b91-443d-a01f-d7ea6b02df96">
## exporting variables
Variables that you set in a shell session are local to that shell process.
When you switch to the subshell (sh), VAR is not passed along because it was not marked as an environment variable. In Unix-like systems, a shell variable only becomes an environment variable (accessible to child processes) if you explicitly export it using the export command.
> flag: (i forgot to export in the start oops) <img width="692" alt="Screenshot 2024-10-11 at 11 19 22 AM" src="https://github.com/user-attachments/assets/0c81d2f5-2910-47a2-b7b5-8f18375e9481">
## printing exported variables
env prints all exported variables in your shell. 
> flag: <img width="742" alt="Screenshot 2024-10-11 at 11 22 10 AM" src="https://github.com/user-attachments/assets/06d57432-614c-48b5-8bc3-51602a0af00f">
## storing comand output
format: VARNAME=$(path)
> flag:<img width="606" alt="Screenshot 2024-10-11 at 11 25 34 AM" src="https://github.com/user-attachments/assets/11855c77-9bbd-49d8-ad57-3ac04b545a10">
## reading input 
read -p "text_to_display: " varname
text_to_display: (entervalhere)
> flag: <img width="559" alt="Screenshot 2024-10-11 at 11 30 40 AM" src="https://github.com/user-attachments/assets/a8f12b24-596c-4f05-8ea9-29d290802762">
## reading files
> flag: <img width="517" alt="Screenshot 2024-10-11 at 11 37 47 AM" src="https://github.com/user-attachments/assets/58e9e3aa-a034-4b9b-9a96-4a9690745322">



