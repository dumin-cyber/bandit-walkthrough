# Bandit Level 8 →9X

## 🎯 Objective

Find the password stored in the file `data.txt`, where the correct password is the only line of text that occurs only once.

## 🔍 Approach

After listing the files with `ls`, I identified `data.txt` and inspected its contents using `cat`. The file contained a large number of seemingly random lines.

Since the password is the only line that appears once, manually reviewing the file would be inefficient. Instead, I used a combination of commands to process the data.

First, I used `sort` to organize all lines. This groups identical lines together, which is necessary for the next step.

Then, I used `uniq -c` to count how many times each line appears. This revealed that most lines were repeated multiple times, while only one line appeared once.

To optimize the process, I used the following command:

```bash
sort data.txt | uniq -u
```

This directly outputs only the unique (non-repeated) lines, making it easy to identify the password.

## 💻 Commands Used

```bash
cat data.txt
sort data.txt | uniq -c
sort data.txt | uniq -u
```

## 🧠 Explanation

* `sort` organizes lines so identical entries are adjacent
* `uniq -c` counts occurrences of each line
* `uniq -u` filters and displays only unique lines

## 📌 Key Takeaways

* Sorting is essential before using `uniq`
* `uniq -u` is efficient for finding non-repeated data
* Processing large datasets requires automation, not manual inspection

## 🧠 Pentesting Insight

In real-world scenarios, large datasets such as logs or dumps often contain repeated information. Identifying unique entries is a powerful technique for uncovering sensitive data like credentials or anomalies.

