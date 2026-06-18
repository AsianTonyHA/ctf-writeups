The password for the next level is stored somewhere on the server and has all of the following properties:

owned by user bandit7
owned by group bandit6
33 bytes in size

immediately i knew that it wasn't just ina obvious directory so i went to root / and did find 
find / -size 33c -user bandit7 -group bandit6 | grep -v "Permission denied"

I aded the grep -v so it would filter out and i was confused on why this didnt work, after soem research
it showed that errors like permission denied get skipped by grep so i would have to add a 2>&1
In linux there are 3 data steams and 2>&1 makes it so errors funnels into the normal output so grep can catch it
and filter normally because without it the errors are in a whole seperate dimension grep can't touch

bandit6@bandit:/$ find / -size 33c -user bandit7 -group bandit6 2>&1 | grep -v "Permission denied"
find: ‘/proc/34/task/34/fd/6’: No such file or directory
find: ‘/proc/34/task/34/fdinfo/6’: No such file or directory
find: ‘/proc/34/fd/5’: No such file or directory
find: ‘/proc/34/fdinfo/5’: No such file or directory
/var/lib/dpkg/info/bandit7.password
bandit6@bandit:/$ cat /var/lib/dpkg/info/bandit7.password
