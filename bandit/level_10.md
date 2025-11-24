# Bandit Level 10


<img width="1538" height="500" alt="download (10)" src="https://github.com/user-attachments/assets/cdf7cbbe-30d7-49e7-b533-724b66670b55" />




## Concept learned
- Searching for strings inside files <br><br>

## Commands used
- grep
- strings [^1] <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit9 and the password you found in the previous level.
2.  The password for the next level is stored in the file data.txt preceded by several '=' characters. To find it use ```strings``` with ```grep```
3.  You first have to find all the human-readable strings with ```strings``` and then filter them using ```grep```:
    ```
    strings data.txt | grep ===
    ```
4.  The output will contain the password. Copy it into your text file and disconnect from the current level.

<br><br><br>

[^1]:[strings man page](https://man7.org/linux/man-pages/man1/strings.1.html)
