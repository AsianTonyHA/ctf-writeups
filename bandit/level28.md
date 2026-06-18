Bandit Level 28 → Level 29
Level Goal
There is a git repository at ssh://bandit28-git@bandit.labs.overthewire.org/home/bandit28-git/repo via the port 2220. The password for the user bandit28-git is the same as for the user bandit28.

From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Commands you may need to solve this level
git

Helpful Reading Material
Installing Git
Git from the Bottom Up
Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN


┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit]
└─$ cd repo

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ ls
README.md

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ cat readme.md
cat: readme.md: No such file or directory

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ cat README.md
# Bandit Notes
Some notes for level29 of bandit.

## credentials

- username: bandit29
- password: xxxxxxxxxx


repo is what installed after: ─$ git clone ssh://bandit28-git@bandit.labs.overthewire.org:2220/home/bandit28-git/repo

