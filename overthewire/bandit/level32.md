Bandit Level 31 → Level 32
Level Goal
There is a git repository at ssh://bandit31-git@bandit.labs.overthewire.org/home/bandit31-git/repo via the port 2220. The password for the user bandit31-git is the same as for the user bandit31.

From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Commands you may need to solve this level
git

Helpful Reading Material
Installing Git
Git from the Bottom Up



┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git push origin master
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit31-git@bandit.labs.overthewire.org's password:
Everything up-to-date

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ ls -la
total 24
drwxr-xr-x  3 lejames lejames 4096 May 24 18:21 .
drwx------ 12 lejames lejames 4096 May 24 18:21 ..
drwxr-xr-x  7 lejames lejames 4096 May 24 18:17 .git
-rw-r--r--  1 lejames lejames    6 May 24 18:17 .gitignore
-rw-r--r--  1 lejames lejames   15 May 24 18:21 key.txt
-rw-r--r--  1 lejames lejames  147 May 24 18:17 README.md

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git log -all
error: switch `l' expects an integer value with an optional k/m/g suffix

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git log --all
commit 955f4b28e0b20807864d79570968cd5ee0baf28a (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:18:00 2026 +0000

    initial commit

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ ls
key.txt  README.md

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git commit -m "gay"
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git add -f key.txt

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git commit -m "gay"
[master d104a25] gay
 1 file changed, 1 insertion(+)
 create mode 100644 key.txt

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$ git push origin master
                         _                     _ _ _
                        | |__   __ _ _ __   __| (_) |_
                        | '_ \ / _` | '_ \ / _` | | __|
                        | |_) | (_| | | | | (_| | | |_
                        |_.__/ \__,_|_| |_|\__,_|_|\__|


                      This is an OverTheWire game server.
            More information on http://www.overthewire.org/wargames

backend: gibson-0
bandit31-git@bandit.labs.overthewire.org's password:
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 326 bytes | 163.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: ### Attempting to validate files... ####
remote:
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote:
remote: Well done! Here is the password for the next level:
remote: 3O9RfhqyAlVBEZpVb6LYStshZoqoSx5K
remote:
remote: .oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.oOo.
remote:
To ssh://bandit.labs.overthewire.org:2220/home/bandit31-git/repo
 ! [remote rejected] master -> master (pre-receive hook declined)
error: failed to push some refs to 'ssh://bandit.labs.overthewire.org:2220/home/bandit31-git/repo'

┌──(lejames㉿DESKTOP-URR1S4O)-[~/repo]
└─$


So basically there was a git commit and it said "key.txt" blah blah blah should have "May I come in?" in it as the comment
and .gitignore had *.txt which is all txt file nuh uh. So if you trie to committ a key.txt file with "May I come in?" 
it doesn't add anything and say it's up to date so you use git add -f key.txt and then comitt then git push origin master
