bandit22@bandit:/etc/cron.d$ cat /usr/bin/cronjob_bandit23.sh
#!/bin/bash
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)

echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"

cat /etc/bandit_pass/$myname > /tmp/$mytarget
bandit22@bandit:/etc/cron.d$

Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: Looking at shell scripts written by other people is a very useful skill. The script for this level is intentionally made easy to read. If you are having problems understanding what it does, try executing it to see the debug information it prints.

Commands you may need to solve this level
cron, crontab, crontab(5) (use “man 5 crontab” to access this)

So the first part is the script and basically grabs tehir user whicb should be bandit23 because it's bandit 23 script
bandit22@bandit:/etc/cron.d$ my name = bandit23
my: command not found
bandit22@bandit:/etc/cron.d$ md5sum I am user bandit23
md5s um: I: No such file or directory
md5sum: am: No such file or directory
md5sum: user: No such file or directory
md5sum: bandit23: No such file or directory
bandit22@bandit:/etc/cron.d$ echo I am user bandit23 | md5sum
8ca319486bfbbc3663ea0fbe81326349  -
bandit22@bandit:/etc/cron.d$ cat /tmp/8ca319486bfbbc3663ea0fbe81326349
0Zf11ioIjMVN551jX3CmStKLYqjk54Ga
bandit22@bandit:/etc/cron.d$
 so basically here i figured out md5sum is a hashing function and since it grabs the first value with
-f 1 in the script 

myname=$(whoami)
mytarget=$(echo I am user $myname | md5sum | cut -d ' ' -f 1)

echo "Copying passwordfile /etc/bandit_pass/$myname to /tmp/$mytarget"

i did just did echo and that into md5suma nd got hte hash and just put that into cat /tmp/hash and got the answer
