# Bandit Level 3 → Level 4

## 🎯 Objective
Find the password stored in a hidden file located inside the `inhere` directory.

## 🔍 Approach
After listing the contents of the current directory using `ls`, I identified a directory named `inhere`.

I navigated into the directory using `cd inhere` and listed its contents. Initially, no files were displayed.

To reveal hidden files, I used the `ls -la` command, which showed additional files including one named `.hidden-file` (in this case: `...Hiding-From-You`).

I then accessed the file to retrieve its password.

## 💻 Commands Used
```bash
ls
cd inhere
ls -la
cat ./...Hiding-From-You
