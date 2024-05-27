# Bandit Level 3 → Level 4

## Level Goal
The password for the next level is stored in a hidden file in the inhere directory.

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit4

### Password
pIwrPrtPN36QITSp3EQaw936yaFoFgAB

## Writeup
Since the password is stored in a file in inhere directory, we will go to inhere directory using <kbd>cd</kbd> ( Change Directory) command.
```bash
cd inhere
```
Now to list all the files including hidden files we will use <kbd>-a</kbd> switch along with <kbd>ls</kbd>
```bash
ls -a
```
In linux OS, hidden file's name begins with a "."
To print the content of <kbd>.hidden</kbd>:
```bash
cat .hidden
```
