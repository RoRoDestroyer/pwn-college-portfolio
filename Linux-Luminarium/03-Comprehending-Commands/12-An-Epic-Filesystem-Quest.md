[An Epic Filesystem Quest]

Module: [Comprehending Commands / Linux Luminarium]

Date: [10/21/2026]

[Objective]:

The first clue is in `/`. Once in look around with `ls`. There'll be a file named HINT or CLUE or something along those lines; `cat` that file to read the clue. Depending on what the clue says, head on over to the next directory, or don't. Follow the clues to the flag.

[Key Concept]:



[Solution]:

To head into `/` we must `cd` into it by writing out: `cd /`. Once in `/` we can look around by writing out `ls`. Many files will show up but the one that sticks out is: `REVELATION`. To read out this file we use `cat` to get the hint: `cat REVELATION`. This will output this: "Tubular find! The next clue is in: /etc/cloud The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'." To enter into this directory we go back to using our `cd` command: `cd /etc/cloud`. Once in we can look around again by using `ls`. This will bring up two files: `TRACE` and `build.info`. `TRACE` looks promising, we can now `cat` out this file: `cat TRACE`. This gives our next clue, it tell us this: "Great sleuthing! The next clue is in: /usr/lib/python3/dist-packages/pwnlib/data/useragents The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'." We know we need to go to the next directory, same as before we can write out: `cd /usr/lib/python3/dist-packages/pwnlib/data/useragents`. The last hint told us the file we are looking for is a hidden file. Knowing this we can use `ls -a` to show hidden files. Doing so outputs these files: `.`, `..`, `.INFO`, `useragents.txt`. Since its a hidden file we know it can't be `useragents.txt`, as it is not a dot prepended file; not hidden. So the next promising one is `.INFO`. We can read this file out now by invoking: `cat .INFO`. This now outputs: "Great sleuthing! The next clue is in: /usr/lib/python3/dist-packages/elftools/elf/__pycache__ Watch out! The next clue is **trapped**. You'll need to read it out without 'cd'ing into the directory; otherwise, the clue will self destruct!" This means we must find the file through the explicit path to avoid self destruction. To do this we can write out: `ls /usr/lib/python3/dist-packages/elftools/elf/__pycache__`. This outputs a handful of files but notably a file named `NUGGET-TRAPPED`. Since we cannot `cd` into this directory, we must also `cat` this file via the explicit path. This would look like: `cat /usr/lib/python3/dist-packages/elftools/elf/__pycache__/NUGGET-TRAPPED`. Doing this correctly gives us our next clue: "Great sleuthing! The next clue is in: /usr/share/man/de/man1" Now we can go into the next directory: `cd /usr/share/man/de/man1`. Then we can look around by using `ls`. This shows tons of files, but notably to the last few formats a file named `SPOILER` stands out. We can read this file now: `cat SPOILER`. This gives us our next clue: "Lucky listing! The next clue is in: /var/lib/apt/lists/auxfiles". Just like the last couple of times we can go to this directory and look; first: `cd /var/lib/apt/lists/auxfiles`; then `ls`. This outputs one file named `MESSAGE`. We can read this file out via: `cat MESSAGE`. This provides us with our next clue: "Tubular find! The next clue is in: /usr/lib/python3/dist-packages/plumbum The next clue is **hidden** --- its filename starts with a '.' character. You'll need to look for it using special options to 'ls'." Once again lets go to this directory: `cd /usr/lib/python3/dist-packages/plumbum`. Since we need to look for  a hidden file that means we need to sue `ls -a` again. This outputs a handful of files again but only one hidden file sticks out, `.DOSSIER'`. We can read this file out: `cat .DOSSIER`. This gives our next clue: "Great sleuthing! The next clue is in: /var/cache/man/uk/cat1 The next clue is **delayed** --- it will not become readable until you enter the directory with 'cd'." We must enter the directory this time with `cd`, we've been doing this so no issue. We can just use our `cd` command again: `cd /var/cache/man/uk/cat1`. Then look around again with `ls`. This outputs one file named `ALERT`, we can read this file out now: `cat ALERT`. We now get our next clue: "Great sleuthing! The next clue is in: /usr/share/man/it" We can of course `cd` into this directory now: `cd /usr/share/man/it`. Then once again look around with `ls`. This will output 4 files, `TIP`, `man1`, `man5`, and `man8`. Following our format, `TIP` looks like the correct file; we can read this out using `cat`: `cat TIP`. That was our last challenge we now get our flag from reading out `TIP`.

[# Relevant command(s) or code]:



[What I Learned]:

The extension of `ls` to view hidden files; `ls -a`. I also learned by default Linux uses a "." notation set at the front of a file name to mark it as hidden.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
