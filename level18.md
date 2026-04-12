
cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3jSo the password I got for 17 was right and I connected, but then it immediately kicked me out of it when i SSH in with the 
right password. x2gLTTjFwMOhQ8oWNbMN362QKxfRqGlO

Level Goal
The password for the next level is stored in a file readme in the homedirectory. Unfortunately, someone has modified .bashrc to log you out when you log in with SSH.

Commands you may need to solve this level
ssh, ls, cat

Since SSH, you can use append a command to the end of a SSH conneciton like this, 

ssh bandit.labs.overthewire.org -p 2220 -l bandit18 "cat readme"

It outputs only that command and nothing like runs because when you try to login with SSH, a script ran that logged me out immediately but with that it only runs cat readme (the password) as stated up there so no logout happens and i get pass for next lvl.

cGWpMaKXVwDUNgPAVJbWYuGHVn9zl3j8
