bandit4@bandit:~$ ls
inhere
bandit4@bandit:~$ cd inhere
bandit4@bandit:~/inhere$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ ls -la
total 48
drwxr-xr-x 2 root    root    4096 Apr  3 15:18 .
drwxr-xr-x 3 root    root    4096 Apr  3 15:18 ..
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file00
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file01
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file02
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file03
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file04
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file05
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file06
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file07
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file08
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file09
bandit4@bandit:~/inhere$ cat -file00
cat: invalid option -- 'f'
Try 'cat --help' for more information.
bandit4@bandit:~/inhere$ cat ./-file00
��y�er`�v>/�ܿa@.�'m�������bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file01
�3��P�WDQ�-^c@�򍣦-�#/Erttbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file02
4t�:Oz�l�)���Lm�L�
                  Y�l��9�0��Mbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file03
��~��ɢ܎Ց��;Kde{f
               +<>�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file04
�-�v��������hH�X��i>*�I�~�aP�8Qbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file05
        VN�F��#��ژ�:է����Vd�Z��כ�#�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file06
o"ُ֛�� ,�i�M�
           -g@x,��v���z�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
bandit4@bandit:~/inhere$ cat ./-file08
��uB�{N����ފ�!-��s��$aA�1mbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file09
�OP�vV�}�H�:�I�%�#�X�
�}�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$

This level had 9 files after ls and one of them happened to contain the flag, but i wanted to know how 
I would have Linux print out a bunch of these inputs at once incase theres like 100 or smthn

bandit4@bandit:~$ ls
inhere
bandit4@bandit:~$ cd inhere
bandit4@bandit:~/inhere$ ls
-file00  -file01  -file02  -file03  -file04  -file05  -file06  -file07  -file08  -file09
bandit4@bandit:~/inhere$ ls -la
total 48
drwxr-xr-x 2 root    root    4096 Apr  3 15:18 .
drwxr-xr-x 3 root    root    4096 Apr  3 15:18 ..
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file00
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file01
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file02
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file03
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file04
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file05
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file06
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file07
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file08
-rw-r----- 1 bandit5 bandit4   33 Apr  3 15:18 -file09
bandit4@bandit:~/inhere$ cat -file00
cat: invalid option -- 'f'
Try 'cat --help' for more information.
bandit4@bandit:~/inhere$ cat ./-file00
��y�er`�v>/�ܿa@.�'m�������bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file01
�3��P�WDQ�-^c@�򍣦-�#/Erttbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file02
4t�:Oz�l�)���Lm�L�
                  Y�l��9�0��Mbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file03
��~��ɢ܎Ց��;Kde{f
               +<>�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file04
�-�v��������hH�X��i>*�I�~�aP�8Qbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file05
        VN�F��#��ژ�:է����Vd�Z��כ�#�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file06
o"ُ֛�� ,�i�M�
           -g@x,��v���z�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file07
4oQYVPkxZOOEOO5pTW81FB8j8lxXGUQw
bandit4@bandit:~/inhere$ cat ./-file08
��uB�{N����ފ�!-��s��$aA�1mbandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$ cat ./-file09
�OP�vV�}�H�:�I�%�#�X�
�}�bandit4@bandit:~/inhere$
bandit4@bandit:~/inhere$

The file was just 10 files and i catted each one and got the flag

