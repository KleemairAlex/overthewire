# Bandit Level 2

<img width="1538" height="500" alt="download (2)" src="https://github.com/user-attachments/assets/fdf49d4b-0f4d-4b11-b200-f87f5a78c2b5" />



## Concept learned
- Handling Files With Special or Problematic Filenames   <br><br>

## Commands used
- ls
- cat   <br><br>

### Walkthrough
1.  Connect to the overthewire host with the username bandit1 and the password you found in the the readme file
2.  After connecting I first looked for the "-" file with ls to make sure it is there
3.  Now read the file content with cat but you can not simply run ```cat -``` since it is a special filename
4.  So to make sure there is no problem one possible solution is to run cat with the whole filepath so the command would be
```
cat ./-
```
5. After running the command you are presented with the next password. Copy it into your text file and disconneting from the current level.


<br><br><br>
> [!TIP]
> To disconnect your current ssh session you simply run ```exit```
