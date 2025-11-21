# Bandit Level 5

<img width="1538" height="500" alt="download (5)" src="https://github.com/user-attachments/assets/d5d04089-012c-4ab2-b75f-ee82761e716c" />



## Concept learned
- Determining file types <br><br>

## Commands used
- ls
- cd
- cat
- file[^1]  <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit4 and the password you found in the the "...Hiding-From-You" file
2.  After connecting, check if the "inhere" directory exist by running ```ls```.
3.  Change into the "inhere" directory with ```cd```.
4.  Search for files with ```ls```. The return will be 10 files. Going through all of them with ```cat``` to try to find the right file is inefficient. A simpler, faster solution is to look for the right file with ```file```.
5.  Running ```file ./*``` will return the file type of every file in the active directory.
6.  Find the file marked as human-readable (e.g., “ASCII text”) read it with ```cat```.
5.  After running ```cat``` you are presented with the next password. Copy it into your text file and disconnect from the current level.

<br><br><br>
[^1]:[file man page](https://manpages.ubuntu.com/manpages/noble/man1/file.1.html)
