┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ nano README.md

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ git log
commit adc7f885a129baee883058b8a870739489f80194 (HEAD -> master, origin/master, origin/HEAD)
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    fix info leak

commit a3437bddd447f2d496731658e86b98cbea9d3c98
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    add missing data

commit cb630ec182b75bc289595511f8bcf4d47cfec50d
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    initial commit of README.md

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ man git

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ git show cb630ec182b75bc289595511f8bcf4d47cfec50d
commit cb630ec182b75bc289595511f8bcf4d47cfec50d
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    initial commit of README.md

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..7ba2d2f
--- /dev/null
+++ b/README.md
@@ -0,0 +1,8 @@
+# Bandit Notes
+Some notes for level29 of bandit.
+
+## credentials
+
+- username: bandit29
+- password: <TBD>
+

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ git show cb630ec182b75bc289595511f8bcf4d47cfec50d
commit cb630ec182b75bc289595511f8bcf4d47cfec50d
Author: Ben Dover <noone@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    initial commit of README.md

diff --git a/README.md b/README.md
new file mode 100644
index 0000000..7ba2d2f
--- /dev/null
+++ b/README.md
@@ -0,0 +1,8 @@
+# Bandit Notes
+Some notes for level29 of bandit.
+
+## credentials
+
+- username: bandit29
+- password: <TBD>
+

┌──(lejames㉿DESKTOP-URR1S4O)-[~/ctf/overthewire/bandit/repo]
└─$ git show a3437bddd447f2d496731658e86b98cbea9d3c98
commit a3437bddd447f2d496731658e86b98cbea9d3c98
Author: Morla Porla <morla@overthewire.org>
Date:   Fri Apr 3 15:17:54 2026 +0000

    add missing data

diff --git a/README.md b/README.md
index 7ba2d2f..d4e3b74 100644
--- a/README.md
+++ b/README.md
@@ -4,5 +4,5 @@ Some notes for level29 of bandit.
 ## credentials

 - username: bandit29
-- password: <TBD>
+- password: 4pT1t5DENaYuqnqvadYs1oE4QLCdjmJ7


So basically when u do git download clone on surface only the head thing is showen, but git always knows what happened before that and 
logs and saves it and each commit has what was in it and a hash so yea pretty easy when just looking at documentatoin and trying commands

