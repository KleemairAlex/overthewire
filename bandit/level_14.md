# Bandit Level 14


<img width="1538" height="500" alt="download (14)" src="https://github.com/user-attachments/assets/144c3cb0-1245-4583-827a-7472933406b4" />








## Concept learned
- SSH keys <br><br>

## Commands used
- ssh
- scp[^1]
- chmod[^2]]<br><br>

### Walkthrough
1. You start by copying the SSH private key file to your local machine using `scp`:
    ```
    scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .
    ```
2. Before using the key, set its permissions so that it is only readable by you:
    ```
    chmod 600 sshkey.private
    ```
3. Connect to Level 14 using the private key:
    ```
    ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
    ```

<br><br><br>

[^1]:[scp man page](https://linux.die.net/man/1/scp)
[^2]:[chmod man page](https://linux.die.net/man/1/chmod)
