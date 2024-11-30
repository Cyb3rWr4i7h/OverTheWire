# Bandit Level 10 → Level 11

## Level Goal
The password for the next level is stored in the file data.txt, which contains base64 encoded data

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit11

### Password
6zPeziLdR2RKNdNYFNb6nVCKzphlXHBM

## Writeup
Here we simply print contents of `data.txt` and decode it through
[CyberChef](https://gchq.github.io/CyberChef/)
using `From Base64`

OR we can do it using command line as:
```bash
 cat data.txt | base64 -d
```
