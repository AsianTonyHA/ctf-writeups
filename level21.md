Bandit Level 21 → Level 22
Level Goal
A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

Commands you may need to solve this level
cron, crontab, crontab(5) (use “man 5 crontab” to access this

tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q

So when visiting /etc/cron.d
one of the scripts shown that ran frequently because of the ***** /usr/bin/cronjob_bandit22.sh

And cat /usr/bin/cronjob_bandit22.sh 
showed chmod 644 /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
cat /etc/bandit_pass/bandit22 > /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
ch mod with 644 meant everyone can read the /tmp/our98hfos directory, and then the second command read /etc/bandit_pass
bandit 22 which only contains the password and redirected it to /tmp, so all i had to do was
bandit21@bandit:/usr/bin$ cat /tmp/t7O6lds9S0RqQh9aMcz6ShpAoZKF7fgv
tRae0UfB9v0UzbCdn9cY0gQnds9GF58Q
bandit21@bandit:/usr/bin$
