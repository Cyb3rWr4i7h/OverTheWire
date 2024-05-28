# Bandit Level 6 → Level 7

## Level Goal
The password for the next level is stored somewhere on the server and has all of the following properties:
  owned by user bandit7
  owned by group bandit6
  33 bytes in size
  
## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit7

### Password
z7WtoNQU2XfjmMtWA8u5rN4vzqu4v99S

## Writeup
Just like previous level, here we will use `find` but with `user` `owner` and `size` option. But in output we receive using `find / -type f -user bandit7 -group bandit6 -size 33c`, to easily look for password, we will remove the lines using `grep` command with `-v` option which will exclude lines containing `Permission denied`.

```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>&1 | grep -v "Permission denied"
```
`2>&1` redirects errors to standard output, so they can be the next command.
