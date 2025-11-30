# Bandit Level 15


<img width="1538" height="500" alt="download (15)" src="https://github.com/user-attachments/assets/b5530749-7321-4588-8e3e-842d0686990c" />






## Concept learned
- Sending input to a port<br><br>

## Commands used
- cat
- nc[^1] <br><br>

### Walkthrough
1.  Connect to this level the same way as described in the walkthrough for Level 14.
2.  At the previous level you don't get the password for this level but you will need it, so start with copying the password from the output of:
    ```
    cat /etc/bandit_pass/bandit14
    ```
3.  Then send the password to port 30000 of localhost using ```nc```:
    ```
    nc localhost 30000
    ```
    After running the command you have to paste the password and press enter.
4.  The output will contain the password for the next level. Copy it into your text file and disconnect from the current level.

<br><br><br>

[^1]:[nc man page](https://linux.die.net/man/1/nc)
