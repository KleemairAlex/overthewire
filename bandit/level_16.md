# Bandit Level 16


<img width="1538" height="500" alt="download (16)" src="https://github.com/user-attachments/assets/c1e033e2-86ee-4183-9e6a-f5d18f4567b6" />







## Concept learned
- Sending input to a port using SSL/TLS<br><br>

## Commands used
- openssl[^1] <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit15 and the password you found in the previous level.
2.  Once logged in, you need to send the current password to a port on localhost, but this time using SSL/TLS encryption:
    ```
    openssl s_client -connect localhost:30001
    ``` 
3.  Parse the current password and hit enter. The output will contain the password for the next level. Copy it into your text file and disconnect from the current level.

<br><br><br>

[^1]:[openssl man page](https://linux.die.net/man/1/openssl)
