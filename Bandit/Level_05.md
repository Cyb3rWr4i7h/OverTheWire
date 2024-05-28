# Bandit Level 5 → Level 6

## Level Goal
The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:
  human-readable
  1033 bytes in size
  not executable
  
## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit6

### Password
P4L4vucdmLnm8I7Vl7jG1ApGSfjYKqJU


## Writeup
Here we will use `find` command  with appropriate options (type, size, readable, non executable) to add the info we know the file. 
```bash
find -type f -size 1033c -readable ! -executable
```
Now we know where the next is present so we can simply print the output using `cat` command.
