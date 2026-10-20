[Hidden Files]

Module: [Comprehending Commands / Linux Luminarium]

Date: [10/20/2026]

[Objective]:

Find the flag, hidden in `/` as a dot-prepended.

[Key Concept]:

Recalling the `ls` command, Linux by default does not show hidden files when you use the basic `ls` command. Noting this, Linux uses a convention that files that start with a "." are hidden. For example, a file named `.hidden` would not show up when using `ls`. To get around this, if you want to view hidden files, you must invoke the `ls` command with a `-a` argument. In full form: `ls -a`.

[Solution]:

To list files and hidden files in `/` run: `ls -a /`. This will output a handful of files, but in particular one stands out: `.flag-24777189867407`. Since this file is the flag we must output this file contents by using `cat`, we can do this by running: `cat /.flag-24777189867407`. This will give our flag.

[# Relevant command(s) or code]:

The `ls` command list files, to extend it into hidden files we can use `ls -a`. The `cat` command reads out files contents into our terminal.

[What I Learned]:

The extension of `ls` to view hidden files; `ls -a`. I also learned by default Linux uses a "." notation set at the front of a file name to mark it as hidden.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
