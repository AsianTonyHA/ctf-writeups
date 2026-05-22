Bandit Level 29 → Level 30
Level Goal
There is a git repository at ssh://bandit29-git@bandit.labs.overthewire.org/home/bandit29-git/repo via the port 2220. The password for the user bandit29-git is the same as for the user bandit29.

From your local machine (not the OverTheWire machine!), clone the repository and find the password for the next level. This needs git installed locally on your machine.

Commands you may need to solve this level
git

Helpful Reading Material
Installing Git
Git from the Bottom Up


┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show 921cad124cfe5b4ba9f648de1894f75656ff0ff4
commit 921cad124cfe5b4ba9f648de1894f75656ff0ff4 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    fix username

diff --git a/README.md b/README.md
index 2da2f39..1af21d3 100644
--- a/README.md
+++ b/README.md
@@ -3,6 +3,6 @@ Some notes for bandit30 of bandit.

 ## credentials

-- username: bandit29
+- username: bandit30
 - password: <no passwords in production!>


┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git log -all
error: switch `l' expects an integer value with an optional k/m/g suffix

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git log --all
commit 921cad124cfe5b4ba9f648de1894f75656ff0ff4 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    fix username

commit 97622e03dcbefc7953e906cecbc8a602f84cba4a (origin/dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add data needed for development

commit b7c20bdb2356159f2645c5c1ae45440bb0b107fa (origin/sploits-dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add some silly exploit, just for shit and giggles

commit edd6383ec473cb45c7f620ad3d762f31ebbc41ea
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    initial commit of README.md

commit 3e3a2f6aa32de4fc5e7eaa9bd53a884e724d9fa5
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add gif2ascii

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git stash list

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git grep password
README.md:- password: <no passwords in production!>

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/dev
  remotes/origin/master
  remotes/origin/sploits-dev

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show 3e3a2f6aa32de4fc5e7eaa9bd53a884e724d9fa5
commit 3e3a2f6aa32de4fc5e7eaa9bd53a884e724d9fa5
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add gif2ascii

diff --git a/code/gif2ascii.py b/code/gif2ascii.py
new file mode 100644
index 0000000..8b13789
--- /dev/null
+++ b/code/gif2ascii.py
@@ -0,0 +1 @@
+

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show b7c20bdb2356159f2645c5c1ae45440bb0b107fa
commit b7c20bdb2356159f2645c5c1ae45440bb0b107fa (origin/sploits-dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add some silly exploit, just for shit and giggles

diff --git a/exploits/horde5.md b/exploits/horde5.md
new file mode 100644
index 0000000..8b13789
--- /dev/null
+++ b/exploits/horde5.md
@@ -0,0 +1 @@
+

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show 97622e03dcbefc7953e906cecbc8a602f84cba4a
commit 97622e03dcbefc7953e906cecbc8a602f84cba4a (origin/dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add data needed for development

diff --git a/README.md b/README.md
index 1af21d3..bc6ad3d 100644
--- a/README.md
+++ b/README.md
@@ -4,5 +4,5 @@ Some notes for bandit30 of bandit.
 ## credentials

 - username: bandit30
-- password: <no passwords in production!>
+- password: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL


┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$
As you can see git log did not work but after reading online documentation I found out that git log --all 
 exists and then one of the things was the password, ez lick.
┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show 921cad124cfe5b4ba9f648de1894f75656ff0ff4
commit 921cad124cfe5b4ba9f648de1894f75656ff0ff4 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    fix username

diff --git a/README.md b/README.md
index 2da2f39..1af21d3 100644
--- a/README.md
+++ b/README.md
@@ -3,6 +3,6 @@ Some notes for bandit30 of bandit.

 ## credentials

-- username: bandit29
+- username: bandit30
 - password: <no passwords in production!>


┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git log -all
error: switch `l' expects an integer value with an optional k/m/g suffix

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git log --all
commit 921cad124cfe5b4ba9f648de1894f75656ff0ff4 (HEAD -> master, origin/master, origin/HEAD)
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    fix username

commit 97622e03dcbefc7953e906cecbc8a602f84cba4a (origin/dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add data needed for development

commit b7c20bdb2356159f2645c5c1ae45440bb0b107fa (origin/sploits-dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add some silly exploit, just for shit and giggles

commit edd6383ec473cb45c7f620ad3d762f31ebbc41ea
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    initial commit of README.md

commit 3e3a2f6aa32de4fc5e7eaa9bd53a884e724d9fa5
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add gif2ascii

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git stash list

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git grep password
README.md:- password: <no passwords in production!>

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git branch -a
* master
  remotes/origin/HEAD -> origin/master
  remotes/origin/dev
  remotes/origin/master
  remotes/origin/sploits-dev

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show 3e3a2f6aa32de4fc5e7eaa9bd53a884e724d9fa5
commit 3e3a2f6aa32de4fc5e7eaa9bd53a884e724d9fa5
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add gif2ascii

diff --git a/code/gif2ascii.py b/code/gif2ascii.py
new file mode 100644
index 0000000..8b13789
--- /dev/null
+++ b/code/gif2ascii.py
@@ -0,0 +1 @@
+

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show b7c20bdb2356159f2645c5c1ae45440bb0b107fa
commit b7c20bdb2356159f2645c5c1ae45440bb0b107fa (origin/sploits-dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add some silly exploit, just for shit and giggles

diff --git a/exploits/horde5.md b/exploits/horde5.md
new file mode 100644
index 0000000..8b13789
--- /dev/null
+++ b/exploits/horde5.md
@@ -0,0 +1 @@
+

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$ git show 97622e03dcbefc7953e906cecbc8a602f84cba4a
commit 97622e03dcbefc7953e906cecbc8a602f84cba4a (origin/dev)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:56 2026 +0000

    add data needed for development

diff --git a/README.md b/README.md
index 1af21d3..bc6ad3d 100644
--- a/README.md
+++ b/README.md
@@ -4,5 +4,5 @@ Some notes for bandit30 of bandit.
 ## credentials

 - username: bandit30
-- password: <no passwords in production!>
+- password: qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL


┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repoforlevel29/repo]
└─$
I found out that git log did not work, butgit log --all did and thats ez lick
 qp30ex3VLz5MDG1n91YowTv4Q8l7CDZL
