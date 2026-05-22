Bandit Level 30 → Level 31
Level Goal
There is a git repository at ssh://bandit30-git@bandit.labs.overthewire.org/home/bandit30-git/repo via the port 2220. The password for the user bandit30-git is the same as for the user bandit30.

From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Commands you may need to solve this level
git

Helpful Reading Material
Installing Git
Git from the Bottom Up


qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git show bd393e0e59a075f92fd84edc0ad8d13f64572de2
commit bd393e0e59a075f92fd84edc0ad8d13f64572de2 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:58 2026 +0000

    initial commit of README.md

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..029ba42
--- /dev/null
+++ b/README.md
@@ -0,0 +1 @@
+just an epmty file... muahaha

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/master

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git checkout master
Already on 'master'
Your branch is up to date with 'origin/master'.

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git checkout HEAD
Your branch is up to date with 'origin/master'.

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git checkout master
Already on 'master'
Your branch is up to date with 'origin/master'.

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git reflog
bd393e0 (HEAD -> master, origin/master, origin/HEAD) HEAD@{0}: checkout: moving from master to master
bd393e0 (HEAD -> master, origin/master, origin/HEAD) HEAD@{1}: checkout: moving from master to master
bd393e0 (HEAD -> master, origin/master, origin/HEAD) HEAD@{2}: clone: from ssh://bandit.labs.overthewire.org:2220/home/bandit30-git/repo

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git tag
secret

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git showtag secret
git: 'showtag' is not a git command. See 'git --help'.

The most similar command is
        shortlog

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$ git show secret
fb5S2xb7bRyFmAvQYQGEqsbhVyJqhnDy

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel30/repo]
└─$
so Git tag is a thing u can add to any commit usually showing version and stuffs
