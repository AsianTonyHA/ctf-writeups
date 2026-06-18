Bandit Level 27 → Level 28
Level Goal
There is a git repository at ssh://bandit27-git@bandit.labs.overthewire.org/home/bandit27-git/repo via the port 2220. The password for the user bandit27-git is the same as for the user bandit27.

From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Commands you may need to solve this level
git

Helpful Reading Material
Installing Git
Git from the Bottom Up



upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB

└─$ git clone ssh://bandit27-git@bandit.labs.overthewire.org:2220/home/bandit27-git/repo
Cloning into 'repo'...
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit27-git@bandit.labs.overthewire.org's password:
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/bandit27]
└─$ ls
repo

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/bandit27]
└─$ cd repo

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/bandit27/repo]
└─$ ls
README

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/bandit27/repo]
└─$ cat readme
cat: readme: No such file or directory

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/bandit27/repo]
└─$ cat README
The password to the next level is: Yz9IpL0sBcCeuG7m9uQFt8ZNpS4HZRcN

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/bandit27/repo]
└─$
