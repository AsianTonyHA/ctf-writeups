Bandit Level 17 → Level 18
Level Goal
There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

Commands you may need to solve this level
cat, grep, ls, diffBandit Level 17 → Level 18
Level Goal
There are 2 files in the homedirectory: passwords.old and passwords.new. The password for the next level is in passwords.new and is the only line that has been changed between passwords.old and passwords.new

NOTE: if you have solved this level and see ‘Byebye!’ when trying to log into bandit18, this is related to the next level, bandit19

Commands you may need to solve this level
cat, grep, ls, diff


bandit17@bandit:~$ man diff
bandit17@bandit:~$ diff --normal passwords.old passwords.new
42c42
< 390zFj2NETFVZkqYw8UEFdN6h40oGVtT
---
> x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO
bandit17@bandit:~$

this was my solving process and took like 10 seconds tops

