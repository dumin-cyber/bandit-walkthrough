# Bandit Level 6 → Level 7

## 🎯 Objective
Find the password for the next level stored somewhere on the server with the following properties:
- owned by user `bandit7`
- owned by group `bandit6`
- 33 bytes in size

## 🔍 Approach
Since the password was stored somewhere on the server, I understood that searching only in the current directory would not be enough.

I used the `find` command starting from the root directory `/` and filtered the search using the conditions provided in the challenge:
- file type
- owner
- group
- size

Because searching across the whole system produces many permission errors, I redirected error output to `/dev/null` to keep the results clean.

## 💻 Commands Used
```bash
find / -type f -user bandit7 -group bandit6 -size 33c 2>/dev/null
