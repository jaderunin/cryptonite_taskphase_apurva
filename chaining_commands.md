## semicolons
Basically, when you hit Enter, your shell executes your typed command and, after that command terminates, give you the prompt to input another command. The semicolon is analogous, just without the prompt and with you entering both commands before anything is executed.
> flag: <img width="729" alt="Screenshot 2024-10-19 at 11 43 15 PM" src="https://github.com/user-attachments/assets/8a6f4b37-4e75-4aef-96c6-d6cfbf3b26da">
## 1st shell script
> flag: 
<img width="833" alt="Screenshot 2024-10-19 at 11 44 21 PM" src="https://github.com/user-attachments/assets/4a48d9f3-75d6-4444-a47b-371dfe964592">
## redirecting:
## executable shell scripts:
When you invoke bash script.sh, you are, of course launching the bash command with the script.sh argument. This tells bash to read its commands from script.sh instead of standard input, and thus your shell script is executed.

It turns out that you can avoid the need to manually invoke bash. If your shell script file is executable (recall File Permissions), you can simply invoke it via its relative or absolute path.
> flag: <img width="674" alt="Screenshot 2024-10-19 at 11 46 42 PM" src="https://github.com/user-attachments/assets/d74790af-ab73-45f4-bfdf-cd8b27a82d7c">
> then i found -rw-r--r-- 1 hacker hacker   18 Oct 18 1:52  y.sh
> then
> <img width="536" alt="Screenshot 2024-10-19 at 11 46 46 PM" src="https://github.com/user-attachments/assets/72c95f9b-6789-48d6-a40d-1aa6b6258cfa">


