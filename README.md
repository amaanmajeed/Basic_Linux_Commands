# Basic Linux Commands

Don't forget to 🌟**Star** the repository, to show your Appreciation and Love.


Linux is the one thing all developers must know by heart. But due to its complications and a not-so-user-friendly UI, not everyone seems to grab the day-to-day concepts. So here is a neat cheat sheet for you. 😇

### Cheat Sheet

__1. ```cd``` command__
 - cd means change directory. You can jump between folders using this command.
 -Syntax: 
   - ```cd <folder_name/path>```
   - ```cd ..``` - to back to the parent folder
   - ```cd ../folder_name``` - 
   - ```cd /<foldername>``` - use absolute paths, which start from the root folder ```/```


__2. ```ls``` command__
 - list command is used to list the files.
 - Syntax: ```ls``` accepts a lot of options 
   - ```ls```
   - ```ls <folder_path>``` - to list files of a specific folder
   -  ```ls -al``` 


__3. ```nano``` command__
 - Syntax:
   - ```nano```
   - ```nano <file_name>``` - to list files of a specific folder
   - ```Ctrl + X```, then press Y (or N for no)


__4. ```mkdir``` command__
 - to create folders
 - Syntax:
   - ```mkdir <folder_name>``` - single folder
   - ```mkdir <folder1> <folder2>``` - multiple folders
   - ```mkdir -p <parentfolder / childfolder>``` - nested folders


__5. ```mv``` command__
 - to move the file and also to rename the file
 - ```mv <from_folder/file> <to_folder/file>``` 
 - ```mv <file1> <file2> <tofolder>``` - to move more than one file, make a list of files and move them to a folder.   


__6. ```man``` command__
 - to get the manual of commands that what specific command actually do and how to use it.
 - Syntax: ```man <command_name>```
 - use ```q``` key to exit from man page


__7. ```touch``` command__
 - to create an empty file
 - Syntax: ```touch <file_name>```
 - If the file already exists, it opens the file in write mode.


__8. ```pwd``` command__
 - prints current folder path.
 
 
__9. ```rmdir``` command__
 - delete __empty__ folders using this command
 - Syntax:
   - ```rmdir <folder_name>```
   - ```rm -rf <folder>``` : _To delete folders with files in them_
   > ❗ NOTE: this command does not ask for the confirmation from the user and immediately remove that you ask it to remove.


__10. ```cp``` command__
 - to copy a file


__11. ```open``` command__
 - to open a file using this command
 - Syntax: ```open <filename>```
  
  
__12. ```find``` command__
 - used to find files or folders matching a particular search pattern. It searches recursively.
 - ```file . -name <file_name>``` - to find the file with its name.
 - Example: to find all the files in the current directory with extension ```.png``` and also print the relative path. 
   - Syntax:
   - ```find . -name '*.png'```


__13. ```alias``` command__
 - to create your command for your convenience.
 - Example: 
   - ```alias ll = 'ls -al'```: use ```ll``` in place of ```ls -al``` command
 - ```alias``` : *(with no option)* to list all alias defines


__14. ```history``` command__
 - shows all the commands that you have used in the past for the current 
terminal session.


__15. ```whoami``` command__
 - Print the current user id and name


__16. ```cat``` command__
 - *SUPER POWERFUL command*
 - ```cat <file_name>``` : prints a file content
 - ```cat <file1> <file2>``` : to print multiple file content
 - ```cat <file1> <file2> > file3``` : to concatenate the content of multiple files into a new one.
 - ```cat <file1> <file2> >> <file3>``` : to append content of multiple files into new one.
 - ```cat <file_name> | <another_command>``` : to feed a file's content as input to another command.
 - ```cat -s <file_name>``` to remove multiple empty lines.


__17. ```wc``` command__
 - helps in counting the lines, words, and characters in a file. Mostly, it is used with pipes ```|``` for counting operation.
 - It will display the number of lines, words, and bytes from the file.
 - Syntax: ```wc [option]... [file]...```


__18. ```sort``` command__
 - used to sort the list items
 - ```sort <file_name>``` : by default case sensitive and alphabetic.
 - ```sort -r <file_name>``` : reverse order sort.
 -  ```sort --ignore-case <file_name>``` : to sort case insensitive, use ```-n``` to sort numerically.
 -  ```sort -u <file_name>``` : to remove duplicated.
 -  Example : ```ls | sort``` : used with the list command.
 

__19. ```chmod``` command__
 - chmod is used to make a file executable and to change the permissions granted to it in Linux
 - ```chmod +x <file_name>``` : make a file executable.
 - ```chmod <permission> <file_name>``` : a set of flags associated with each file determines who can access that file, and how they can access it.
 -  Example : ```chmod 755 main.py | chmod +x main.py``` : used to make the file `main.py` executable.


__20. ```locate``` command__
- used to locate a file in a Linux system, just like the search command in Windows.
- useful when you don't know where a file is saved or the actual name of the file.
- ```locate -i hello```: -i argument with the command helps to ignore the case, will also fetch files with Hello or HELLO or heLLo etc.
- ```locate -i *hello*world*```: * helps you to find the files if you remember only some words of the filename, separate them with *, for ex here linux will find any filename with the words "hello" and "world" in them.


__21. ```clear``` command__
 - used to clear the terminal screen
 - useful when you want to declutter your terminal window
 - Syntax: ```clear```
 - Keyboard shortcut: `Ctrl + L` 


__22. ```echo``` command__
 - used to input text and display it on standard output
 - used to print files of a specific kind : ```echo *.svg``` or simply `echo *` to list out the files in the current directory
 - Syntax: ```echo <option(s)> <string(s)>```
 - > 💡 NOTE: The ‘-e‘ option in Linux acts as an interpretation of escaped characters that are backslashed.
 - Example: ```echo -e "\vMr. \vStark \vI \vdon't \vfeel \vso \vgood."```: \v creates vertical tab spaces.



---
*Don't forget to 🌟**Star** the repo, and show your LOVE. 👏