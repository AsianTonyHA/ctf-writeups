Bandit Level 32 → Level 33
Level Goal
After all this git stuff, it’s time for another escape. Good luck!

Commands you may need to solve this level
sh, man


So getting in puts you in a shell that you can only do uppercase letters in. I tried doing special syntax like ./ and stuffs
but I gave up, I legit could not do it, 1 hour of straight spamming shit and trying to find patterns in this shell made me go crazy. And the sol
ution was $0, which is a command that represents the current shell, and when you run $0 it causes the shell to switch back to the original normal
shell and not the broken one, so it becomes normal again.

Once in the normal shell 

whoami
bandit33 (the current level is bandit 32)

so moving to cd /etc/bandit_pass and reading bandit33 password gives tQdtbs5D5i2vJwkO8mEyYEyTL8izoeJ0
