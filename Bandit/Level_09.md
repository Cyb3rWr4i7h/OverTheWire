# Bandit Level 9 → Level 10

## Level Goal
The password for the next level is stored in the file data.txt in one of the few human-readable strings, preceded by several ‘=’ characters.

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit10

### Password
G7w8LIi6J3kTb8A7j9LgrywtEUlyyp6s

## Writeup
To get all the strings present in a file, we can use `strings` command, then we can simply `grep` the lines starting from `==` (Since it mentions several "=" characters, it would have at least two to rule out some extra lines 😎😎)

```bash
strings data.txt | grep ^==
```
