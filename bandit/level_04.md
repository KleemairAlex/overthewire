# Bandit Level 4

<img width="1538" height="500" alt="download (4)" src="https://github.com/user-attachments/assets/d2702903-3f9f-4893-acd2-fedc0b669b17" />




## Concept learned
- Discovering hidden files <br><br>

## Commands used
- ls
- cat
- cd[^1]  <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit3 and the password you found in the "--spaces in this filename--" file
2.  After connecting, check if the "inhere" directory exist by running ```ls```.
3.  Change into the "inhere" directory with ```cd``` which stands for change directory. The full command is cd <directory-name>, where the directory becomes your new active directory.
4.  Next you start with searching for files with ```ls```, which won't return anything because the file you are looking for is hidden.
5.  So to find hidden files, run ```ls -a```.  (literally _list -all_)
6.  Read the hidden file content with ```cat```.
7.  After running ```cat``` you are presented with the next password. Copy it into your text file and disconnect from the current level.

<br><br><br>
> [!NOTE]
> Files or directories with names beginning with a dot (.) are considered hidden. These are often configuration files or system settings that users typically don't need to see or interact with daily.
[^1]:[cd man page](https://manpages.ubuntu.com/manpages/noble/man1/cd.1posix.html)
