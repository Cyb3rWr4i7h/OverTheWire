# Bandit Level 11 → Level 12

## Level Goal
The password for the next level is stored in the file data.txt, where all lowercase (a-z) and uppercase (A-Z) letters have been rotated by 13 positions

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit12

### Password
JVNBBFSmZwKKOP0XbFXOoW8chDz5yVRv

## Writeup
We can print the content of data.txt using `cat` command and we can the ROT13 operation on ![CyberChef](https://cyberchef.org/#recipe=ROT13(true,true,false,13)) over this data or we can use the `tr` (translate) command as:
```bash
cat data.txt | tr 'A-Za-z' 'N-ZA-Mn-za-m'
```
