Bandit Level 12 → Level 13
Level Goal
The password for the next level is stored in the file data.txt, which is a hexdump of a file that has been repeatedly compressed. For this level it may be useful to create a directory under /tmp in which you can work. Use mkdir with a hard to guess directory name. Or better, use the command “mktemp -d”. Then copy the datafile using cp, and rename it using mv (read the manpages!)

Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd, mkdir, cp, mv, file

Helpful Reading Material

I strugged on this level majorly, i first created a temporary directory and copied the .txt into the temp
directory like it told me to and then after I tried the different decompressing commands but none of them 
worked. Even if I manually changed file extensions.

I read documentation prodivded and it said that the decompression tools wont work if the file 
is in hexdump format, so I reverted the hexdump and the file command said it was a gzip file
I decompressed it and it said it was a bzip2 file, then tar, and it kept doing this for a little bit
and then I got  The password is: FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn 
