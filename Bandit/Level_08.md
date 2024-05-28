# Bandit Level 8 → Level 9

## Level Goal
The password for the next level is stored in the file data.txt and is the only line of text that occurs only once

## Box and Port
bandit.labs.overthewire.org:2220

### Username
bandit9

### Password
EN632PlfYiZbn3PhVK3XOGSlNInNE00t

## Writeup
We will use `uniq` command with `-c` option to prefix the lines by their number of occurences. But uniq only counts occurences in consecutive lines so first we will sort the file using `sort` command. Then we can use `sort` again to get the lines sorted in their order of recurrence and finally the first line using `head` or we can use `grep` to get the line starting with `1`, since line containing password is only line repeated once.


```bash
 sort data.txt | uniq -c | sort | head -1
```

Using `grep`:
```bash
sort data.txt | uniq -c | grep ^1
```
