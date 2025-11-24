# Bandit Level 9

<img width="1538" height="500" alt="download (9)" src="https://github.com/user-attachments/assets/dac55e48-1136-4bf2-bc41-09d655f5773a" />




## Concept learned
- Identifying unique lines in a file <br><br>

## Commands used
- sort[^1]
- uniq[^2]  <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit8 and the password you found in the previous level.
2.  The password is like in the last level in the data.txt file. But this time you can't use ```grep``` because you are not looking for a specific text. You need to find the only line of text that occurs only once. To locate the password you have to use ```sort``` and ```uniq```.
3.  Run:
    ```
    sort data.txt | uniq -u
    ```
    ```sort``` groups identical lines together, and ```uniq -u``` prints only the lines that occur once.
4.  After running the command you are presented with the next password. Copy it into your text file and disconnect from the current level.

<br><br><br>
[^1]:[sort man page](https://man7.org/linux/man-pages/man1/sort.1.html)
[^2]:[uniq man page](https://man7.org/linux/man-pages/man1/uniq.1.html)
