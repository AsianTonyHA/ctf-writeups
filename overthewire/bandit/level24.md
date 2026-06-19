gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8
Bandit Level 24 → Level 25
Level Goal
A daemon is listening on port 30002 and will give you the password for bandit25 if given the password for bandit24 and a secret numeric 4-digit pincode. There is no way to retrieve the pincode except by going through all of the 10000 combinations, called brute-forcing.
You do not need to create new connections each time


bandit24@bandit:~$ nc localhost 30002
I am the pincode checker for user bandit25. Please enter the password for user bandit24 and the secret pincode on a single line, separated by a space.
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 1239
Wrong! Please enter the correct current password and pincode. Try again.
gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 1240
Wrong! Please enter the correct current password and pincode. Try again.

Each time you don't have to do another NC
#!/bin/bash

for i in $(seq 0000 9999); do
    echo "gb8KRRCsshuZXI0tUuR6ypOFjiZbf3G8 $i"
done | nc localhost 30002

this is my script it basically just echo a buncha times then force feeds nclocalhost 30002

Wrong! Please enter the correct current password and pincode. Try again.
Wrong! Please enter the correct current password and pincode. Try again.
Wrong! Please enter the correct current password and pincode. Try again.
Wrong! Please enter the correct current password and pincode. Try again.
Wrong! Please enter the correct current password and pincode. Try again.
Wrong! Please enter the correct current password and pincode. Try again.
Correct!
The password of user bandit25 is iCi86ttT4KSNe1armKiwbQNmB3YJP3q4

this was after alot of wrong!
i could've piped it into a file and grepped but no fun in that

and after sshing in with bandit 25
bandit26:x:11026:11026:bandit level 26:/home/bandit26:/usr/bin/showtext
this is for bandit 26

after this i searched up what usr bin showtext was and it's a thing that makes it so it shows a text file with
a more, and with more you can't continue unless its been continued or canceled so if u made ur screen small
it would force more

I had to ask AI what to do after this cus cuh i could not figure it out and it said to use VIM and I did and
typed in the commands needed to get into Bash from Vim, it was very confusing even with AI help
after doing it i had bash
then 
bandit26@bandit:~$ ./bandit27-do
Run a command as another user.
  Example: ./bandit27-do id
bandit26@bandit:~$ ./bandit27-do cat /etc/bandit_pass/bandit27
upsNCc7vzaRDx6oZC6GiR6ERwe1MowGB
bandit26@bandit:~$ ls
bandit27-do  text.txt
bandit26@bandit:~$
bandit27-do is a setuid thing so this took 5 seconds
