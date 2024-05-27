# Bandit Level 2 → Level 3

## Level Goal
The password for the next level is stored in a file called spaces in this filename located in the home directory

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit3
### Password
UmHadQclWmgdLOKQ3YNgjWxGoRMb5luK

## Writeup
In using cat with multiple space separated words, cat will treat them as different filename and concatenate their content. To print the content of spaces in this filename we will use: 
```bash
cat "spaces in this filename"
```
