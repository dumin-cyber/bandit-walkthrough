# Bandit Level 0 → Level 1

## 🎯 Objective
Find the password for the next level stored in a file named `readme` within the home directory.

## 🔍 Approach
After gaining access to the system, I performed basic enumeration to identify available files.

Using the `ls` command, I listed the contents of the current directory and discovered the file named `readme`.

I then accessed the file to retrieve its contents through the `cat` command.

## 💻 Commands Used
```bash
ls
cat
