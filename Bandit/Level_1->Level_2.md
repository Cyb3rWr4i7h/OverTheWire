# Bandit Level 1 → Level 2

# Level Goal
The password for the next level is stored in a file called - located in the home directory

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit2
### Password
rRGizSaX8Mk1RTb1CNQoXTcYZWU6lgzi

## Writeup
The <kbd>-</kbd> is used as a special argument in linux based OS. It is used for standard input and output. When used with commands that read input such as cat, it signifies that input should be taken from stdin.
So to display the contents of filenamed <kbd>-</kbd>, we use:
```bash
cat ./-
```
