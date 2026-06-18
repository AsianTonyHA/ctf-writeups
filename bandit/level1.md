Level 1 after Bandit 0

Intially when you get into SSH, there is just a file named -

I tried intially cat the file, but did not work

I tried to look through different directories by going through to root directory but that seemed out of scope

I then looked at documentation for the cat command, and realized that whenever you wanted to add a 
extra step to a command, you do - like with ls -la, so I searched up how to make Linux search up for things
with the name -, and it said ./- would make it so I would be able to search for that, this is because ./ forces 
things to be a path not an extra step.

After of which cat ./- provided me with 263JGJPfgU6LtdEvgfWU1XP5yac29mFx which was the flag for bandit2


