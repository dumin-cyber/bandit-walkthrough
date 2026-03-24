# Bandit Level 2 → Level 3

## 🎯 Objective
Find the password stored in a file named `--spaces in this filename--` located in the home directory.

## 🔍 Approach
After listing the contents of the directory using `ls`, I identified the target file.

My initial attempt was to access the file using `cat ./--spaces in this filename--`, but this failed due to the presence of spaces in the filename.

To correctly reference the file, I enclosed the filename in quotes so it would be interpreted as a single argument.

## 💻 Commands Used
```bash
ls
cat "./--spaces in this filename--"
