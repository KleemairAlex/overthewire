# Bandit Level 8


<img width="1538" height="500" alt="download (8)" src="https://github.com/user-attachments/assets/4f65d72b-d51c-4852-bb64-a6ff5254e8e6" />





## Concept learned
- Searching for text inside files <br><br>

## Commands used
- grep[^1]  <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit7 and the password you found in the previous file.
2.  The password for the next level is stored in the file data.txt next to the word "millionth". To find it you use ```grep``` which finds text in files
3.  The command is very simple:
    ```
    grep millionth data.txt
    ```
4.  After running ```grep``` you are presented with the next password in the line next to "millionth". Copy it into your text file and disconnect from the current level.

<br><br><br>

[^1]:[grep man page](https://manpages.ubuntu.com/manpages/noble/man1/grep.1.html)
