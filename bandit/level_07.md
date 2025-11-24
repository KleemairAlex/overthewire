# Bandit Level 7


<img width="1538" height="500" alt="download (7)" src="https://github.com/user-attachments/assets/b04960cc-39eb-4e88-b25b-cc232b346e7d" />




## Concept learned
- Searching for files based on specific properties <br><br>

## Commands used
- cat
- find  <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit6 and the password you found in the previous file.
2.  The password for the next level is stored somewhere in the server. You need to find a file which meets these criteria:
     - The owner must be user bandit7
     - Must be owned by group bandit6
     - It is exactly 33 bytes in size
      
3.  So the find command would be:
    ```
    find / -user bandit7 -group bandit6 -size 33c 
    ```
4. The command is correct but it has a problem - the output will be full of permission denied errors since you are searching system wide directories you do not have access to. To avoid these errors simply add ```2>/dev/null``` to the find command.
5. Read the file that match the criteria using ```cat```.
6. Copy the password into your text file and disconnect from the current level.
   

<br><br><br>
>[!NOTE]
>```2>/dev/null``` redirects error messages (stderr) into /dev/null, which discards them.
This prevents “Permission denied” messages from cluttering the output when using find to search system-wide directories.
