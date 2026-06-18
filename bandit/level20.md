0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
Bandit Level 20 → Level 21
Level Goal
There is a setuid binary in the homedirectory that does the following: it makes a connection to localhost on the port you specify as a commandline argument. It then reads a line of text from the connection and compares it to the password in the previous level (bandit20). If the password is correct, it will transmit the password for the next level (bandit21).

NOTE: Try connecting to your own network daemon to see if it works as you think

Commands you may need to solve this level
ssh, nc, cat, bash, screen, tmux, Unix ‘job control’ (bg, fg, jobs, &, CTRL-Z, …)

So basically in the thing ./suconnect Usage: ./suconnect <portnumber>
This program will connect to the given port on localhost using TCP. If it receives the correct password from the other side, the next password is transmitted back.

and if the ./suconnect recieves the password of the previous level and sends it to that port, it will send back that 
next level password, and in this case I has to learn what a network daemon is, so basically it's a thing that runs
in the background waititing for network requests to come and adds it's thing to it

bandit20@bandit:~$ echo 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO|nc -l -p 6969 &
[1] 258
bandit20@bandit:~$ jobs
[1]+  Running                 echo 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO | nc -l -p 6969 &
bandit20@bandit:~$ ./suconnect 6969
Read: 0qXahG8ZjOVMN9Ghs7iOWsCfZyXOUbYO
Password matches, sending next password
EeoULMCra2q0dSkYj561DX7s1CpBuOBt
bandit20@bandit:~$

learned that & keeps things running in background and stuff and jobs lets u see background proccesses 
