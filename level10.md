Bandit Level 10 → Level 11
Level Goal
The password for the next level is stored in the file data.txt, which contains base64 encoded data
dtR173fZKb0RRsDFSGsg2RWnpNVj3qRr
Commands you may need to solve this level
grep, sort, uniq, strings, base64, tr, tar, gzip, bzip2, xxd

Helpful Reading Material
Base64 on Wikipedia


base64 -d data.txt

Since the file is just a short piece of base 64you could use base64 to just decode it
