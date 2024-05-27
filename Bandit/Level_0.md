# Bandit Level 0

## Level Goal

The goal of this level is for you to log into the game using SSH. The host to which you need to connect is bandit.labs.overthewire.org, on port 2220. The username is bandit0 and the password is bandit0. Once logged in, go to the Level 1 page to find out how to beat Level 1.


## Box and Port
bandit.labs.overthewire.org:2220

## Writeup
<kbd>ssh</kbd> command is used to establish a secure shell connection. The correct systax is:
<kbd>ssh username@hostname -p port-number</kbd>. By default the port number is 22 but here to connect to port number 2220 so we specify it using -p.

```bash
ssh bandit0@bandit.labs.overthewire.org -p 2220
```
After putting this command you will be prompted for password: bandit0
