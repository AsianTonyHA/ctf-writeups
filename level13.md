Bandit Level 13 → Level 14
Level Goal
The password for the next level is stored in /etc/bandit_pass/bandit14 and can only be read by user 
bandit14. For this level, you don’t 

get the next password, but you get a private SSH key that can be used to log 
into the next level. Look at the commands that logged you into previous bandit levels, and find out how to use 
the key for this level.

Commands you may need to solve this level
ssh, scp, umask, chmod, cat, nc, install

Helpful Reading Material
SSH/OpenSSH/

scp -P 2220 bandit13@bandit.labs.overthewire.org:/home/bandit13/sshkey.private ~/ctf/
overthewire/bandit/sshkey.privatescp -P 2220 
bandit13@bandit.labs.overthewire.org:/home/bandit13/sshkey.private ~/ctf/ove
rthewire/bandit/sshkey.private


used this command to get the SSH private key from bandit 13 to my Kali terminal 

I then tried to use my by just doing -i and then the directory of the private key file but it said bad perms
and reading at documentaton says that it too open and it should be 600 so read and wwrite for owner no one else tho

after that it worked and i got to level 14, 
