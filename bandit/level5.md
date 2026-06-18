The The password for the next level is stored in a file somewhere under the inhere directory and has all of the following properties:

human-readable
1033 bytes in size
not executable

With the level hacing 20 irectories with multiple files in each, searching for them one by one is too long

First thing I did is how to search like everything and if i do ./*/* it searches all directories then the files
in the directories 
But I tried some stuffs but I was using the file command which oesn't help me too mcuh so i started
reading ocumentation on the find command and it said that find ./ serches for everything eveyrhting so i did that 
and then the size requirement of 1033c (1033 bytes) because the person said its exactly 1033 bytes in size and there 
wenre 100 files like that and there was just one and it was the flag 

bandit5@bandit:~/inhere$ find ./ -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$ find ./*/* -size 1033c
bandit5@bandit:~/inhere$ find ./* -size 1033c
./maybehere07/.file2
bandit5@bandit:~/inhere$

Having it search 2 things deep doesn't work becasue theres nothing 2 things deepfor it to search 
HWasnPhtq9AVKe0dmk45nxy20cvUa6EG 
