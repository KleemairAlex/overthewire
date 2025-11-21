# Bandit Level 6

<img width="1538" height="500" alt="download (6)" src="https://github.com/user-attachments/assets/f8d09cb8-ff09-4900-8444-321826dfa16d" />




## Concept learned
- Searching for files based on specific properties <br><br>

## Commands used
- ls
- cd
- cat
- find[^1]  <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit5 and the password you found in the previous file
2.  After connecting, check if the "inhere" directory exists by running ```ls```.
3.  Change into the "inhere" directory with ```cd```.
4.  Search for files with ```ls```. You will see 20 directories each filled with multiple files. 
5.  To find the needed file you have to use ```find``` and specify the properties that overthewire tells you.
    1. The first criteria is human-readable, which we cannot directly filter with find
    2. The second criteria is that the file must be 1033 bytes in size, which can be filtered using ```-size 1033c``` (```c``` means bytes).
    3. The third criteria is that it must not be executable which we filter with ```! -executable```
6.  So the whole command would be:
   ```
    find . -type f -size 1033c ! -executable
   ```
7.  Read the file with ```cat```.
8.  The file contains the password for the next level. Copy it into your text file and disconnect from the current level.

<br><br><br>
>[!NOTE]
>The ```-type f``` option ensures that ```find``` only looks for files, while the leading ```.``` tells ```find``` to start searching in the current directory and include all subdirectories.
[^1]:[find man page](https://manpages.ubuntu.com/manpages/noble/man1/find.1.html)
