[Home Sweet Home]

Module: [Pondering Paths / Linux Luminarium]

Date: [9/02/2026]

[Objective]:

`/challenge/run` will write a copy of the flag to any file specified, the argument is your path to the file. Your argument must be an absolute path, the path must be inside your home directory, before expansion, your argument must be three characters or less.

[Key Concept]:

Every user has a home directory, typically labeled as `/home`, the home directory is where most users store their personal files. The `~` signifies the users directory, for example, `/home/user`. This means bash takes `~` and signifies it as a shorthand for the user's home directory path.

[Solution]:

Since on bash startup automatically loads us into our home directory, signified by `~$` we can immediately start off by creating our file. For this we will use `touch h`, then we will invoke the command with our argument: `/challenge/run ~/h`. This will finish the challenge and the challenge will then read out the flag to terminal, thus completing it.

[# Relevant command(s) or code]:

The `touch` command creates files, and the subsequent argument will be the name of the file created. (prior knowledge, this lesson did NOT teach this). `~` is a shortcut for the user's home directory `/home/user/`

[What I Learned]:

The `~` signifies the user is in their home directory. Home directory typically stores the users personal files.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
