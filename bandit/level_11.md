# Bandit Level 11


<img width="1538" height="500" alt="download (11)" src="https://github.com/user-attachments/assets/2c7c48d3-b9a8-491d-8f06-f80446844ec4" />





## Concept learned
- Decoding Base64 from the command line<br><br>

## Commands used
- base64[^1] <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit10 and the password you found in the previous level.
2.  The password is once again hidden in data.txt. This time you don't have to search for password - it is right there when you run ```cat data.txt``` but the problem is that it is Base-64-encoded.
3.  So decode it using ```base64```:
    ```
    base64 -d data.txt 
    ```
    -d stands for decode
4.  The decoded output will contain the password. Copy it into your text file and disconnect from the current level.

<br><br><br>

[^1]:[base64 man page](https://man7.org/linux/man-pages/man1/base64.1.html)
