# Bandit Level 17


<img width="1538" height="500" alt="download (17)" src="https://github.com/user-attachments/assets/58ed1a69-69b9-4ebb-b26b-c6c955c48995" />








## Concept learned
- Port scanning a range of ports
- Detecting SSL/TLS services<br><br>

## Commands used
- openssl
- nmap[^1] <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit16 and the password you found in the previous level.
2.  Use nmap with service detection to identify which port is running an SSL/TLS service:
    ```
    nmap -sV -p 31000-32000 localhost
    ```
3.  From the scan results, find the single port that shows an SSL-enabled service. Connect to it using OpenSSL:
    ```
    openssl s_client -connect localhost:31790 -ign_eof
    ```
4. When the connection opens, paste the current password and press Enter. The server will return the SSH key for the next level. Copy into a new SSH key file or the sshkey.private you used last time.

<br><br><br>
>[!NOTE]
>You have to use ```-ign_eof``` so openssl s_client doesn’t quit when you send the password. This keeps the connection open and avoids a keyupdate that would stop the server from receiving it.
[^1]:[nmap man page](https://linux.die.net/man/1/nmap)
