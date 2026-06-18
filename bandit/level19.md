Bandit Level 19 → Level 20
Level Goal
To gain access to the next level, you should use the setuid binary in the homedirectory. Execute it without arguments to find out how to use it. The password for this level can be found in the usual place (/etc/bandit_pass), after you have used the setuid binary.

Helpful Reading Material
setuid on Wikipedia

Setuid is basically a temporary thing when you run something you run as the owner of the filer instead of you

bandit19@bandit:~$ ./bandit20-do
Run a command as another user.
  Example: ./bandit20-do whoami
bandit19@bandit:~$ ./bandit20-do whoami
bandit20


/home/bandit19/bandit20-do cat bandit20
So basically the first part before cat bascially means I am bandit 20 and since i need bandit20 perms to read bandit 20
password in this directory /etc/bandit_pass it works; 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
