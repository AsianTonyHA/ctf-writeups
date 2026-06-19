Bandit Level 14 → Level 15
Level Goal
The password for the next level can be retrieved by submitting the password of the current level to port 30000 on localhost.

Commands you may need to solve this level
ssh, telnet, nc, openssl, s_client, nmap

Helpful Reading Material
How the Internet works in 5 minutes (YouTube) (Not completely accurate, but good enough for beginners)
IP Addresses
IP Address on Wikipedia
Localhost on Wikipedia
Ports
Port (computer networking) on Wikipedia


I first got the password form previous level cus it said the pass for 14 is 
MU4VWeTyJk8ROof1qqmcBPaLh7lDCPvS but only level 14 had the perms to look, but it says here all i need to do
is subit that password into port 30 on localhost

The documentation provided says that the nc command can connect to ports and send and recieve information,
and the localhost in this scenario is not my computer but the server's because im connecting via SSH
so im really just sending a question and getting an answer from myself
so with the command echo (password) | nc localhost 30000 i got 
Correct!
8xCjnmgoKbGLhHFAZlGE5Tmu4M2tKJQo
