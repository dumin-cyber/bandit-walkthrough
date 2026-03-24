# Bandit Level 5 → Level 6

## 🎯 Objective
Find the password stored in the only human-readable file within the `inhere` directory.

## 🔍 Approach
After listing the contents of the current directory, I identified a directory named `inhere` and navigated into it.

Inside the directory, multiple files were present, all starting with a hyphen (`-`), which can be interpreted as command-line options.

To efficiently identify the correct file, I used the `file` command to determine the type of each file. However, using `file *` directly may cause issues because filenames starting with `-` can be interpreted as flags.

To avoid this, I explicitly referenced the current directory using `./*`.

## 💻 Commands Used
```bash
ls
cd inhere
ls
file ./*
cat ./-file07
