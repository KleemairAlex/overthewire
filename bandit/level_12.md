# Bandit Level 12



<img width="1538" height="500" alt="download (12)" src="https://github.com/user-attachments/assets/dcded585-452e-4a45-b5f1-f4f25782334e" />






## Concept learned
- Decoding ROT13 decryption <br><br>

## Commands used
- cat
- tr[^1] <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit11 and the password you found in the previous level.
2.  Just like in level 11 the password is stored in data.txt but with another encryption method called ROT13.
3.  To decode ROT13 encoded text use ```tr```:
    ```
    cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m' 
    ```
4.  The decoded output will contain the password. Copy it into your text file and disconnect from the current level.

<br><br><br>

[^1]:[tr man page](https://man7.org/linux/man-pages/man1/tr.1.html)
