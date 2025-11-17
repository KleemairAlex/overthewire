# Bandit Level 0

<img width="1538" height="500" alt="download" src="https://github.com/user-attachments/assets/cacbe71f-57d1-4327-bf6e-fc9bc5a9fc28" />

## Concept learned
- Secure remote access with ssh  <br><br>

## Commands used
- ssh[^1]  <br><br>

### Walkthrough
So to connect to the overthewire host of the first level **you can _not_ just run**
```
ssh bandit.labs.overthewire.org 
```
You also need a username so the exact level can be clarified. 
To clarify the username simply write the username with an @ before the host. You also need to clarify the port to which you want to connect to. The port can be specified by adding ```-p "portnumber"``` after the host. 
So the full command looks like this:
```
ssh username@host -p port
```
After hitting enter you are prompted for the password which is provided on the [overthewire website](https://overthewire.org/wargames/bandit/bandit0.html).

<br><br><br>

> [!TIP]
> With the command ```man``` you can find out what new commands do (e.g. ```man ssh``` shows the manual for ssh).

[^1]:[Secure shell Wikipedia page](https://en.wikipedia.org/wiki/Secure_Shell)
