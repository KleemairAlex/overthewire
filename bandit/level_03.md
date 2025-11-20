# Bandit Level 3

<img width="1538" height="500" alt="download (3)" src="https://github.com/user-attachments/assets/19a1fe08-1116-4a5d-bf2a-5a9820b79d08" />



## Concept learned
- Handling Files With Special or Problematic Filenames <br><br>

## Commands used
- ls 
- cat  <br><br>

### Walkthrough
The third level is similiar to the second level.
1.  Connect to the overthewire host with the username bandit2 and the password you found in the the "-" file
2.  After connecting I first looked for the "--spaces in this filename--" file with ```ls``` to make sure it is there
3.  Now read the file content with ```cat``` but you can not simply run ```cat ./--spaces in this filename--``` like in the last level since running this would throw an error.
4.  Filenames with spaces must be written in quotes so the shell treats the entire name as one argument instead of splitting it into separate words. So the command for "--spaces in this filename--" would be:
```
cat ./"--spaces in this filename--"
```
5. After running the command you are presented with the next password. Copy it into your text file and disconneting from the current level.

<br><br><br>
