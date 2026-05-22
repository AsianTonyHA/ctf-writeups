
Bandit Level 25 → Level 26
Level Goal
Logging in to bandit26 from bandit25 should be fairly easy… The shell for user bandit26 is not /bin/bash, but something else. Find out what it is, how it works and how to break out of it.

NOTE: if you’re a Windows user and typically use Powershell to ssh into bandit: Powershell is known to cause issues with the intended solution to this level. You should use command prompt instead.

Commands you may need to solve this level
ssh, cat, more, vi, ls, id, pwd

So bascially for this level 
cat /etc/passwd | grep bandit26
# Saw /usr/bin/showtext as the shell
to check for shell
cat /usr/bin/showtext
# Saw it uses "more" to display a file

also displayed home directory in the etc/passwd
Step 3 — Make terminal tiny

Dragged terminal window to be very small
This forces more to pause instead of exiting

ssh -i bandit26.sshkey bandit26@localhost -p 2220
# more paused because terminal too small

:set shell=/bin/bash
:shell

Use Vim



cat /etc/bandit_pass/bandit27
because there was a SETUID and i just used that with this to read the password
