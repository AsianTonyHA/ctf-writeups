Bandit Level 15 → Level 16
Level Goal
The password for the next level can be retrieved by submitting the password of the current level to port 30001 on localhost using SSL/TLS encryption.

Helpful note: Getting “DONE”, “RENEGOTIATING” or “KEYUPDATE”? Read the “CONNECTED COMMANDS” section in the manpage.

Commands you may need to solve this level
ssh, telnet, nc, ncat, socat, openssl, s_client, nmap, netstat, ss

Helpful Reading Material

This level is relatively simple as it's basically jsut the previous one using the nc command
but now using the openssl thing which is a big toolkit for encyptoin
NC sends shi with 0 encryption so any one listening in can get all passwords
openssl does nothing its just like a big overall client, and then s_client is a specific tool in that toolkit
that does SSL/TLS encryption over the connectino 

I tried doing localhost 30001 after that but didnt work because it needs more syntax with -connect
and the localhost:30001 and then it gave me some big ahh response, and then searched it up and using the flag
-quiet removes all the certificate gibberish nonsense and got the flag
kSkvUpMQ7lBYyCM4GBPvCvT1BfWRy0Dx


