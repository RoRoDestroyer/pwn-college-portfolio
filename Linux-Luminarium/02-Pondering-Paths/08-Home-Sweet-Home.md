[Home Sweet Home]

Module: [Pondering Paths / Linux Luminarium]

Date: [9/02/2026]

[Objective]:

`/challenge/run` will write a copy of the flag to any file specified, the argument is your path to the file. Your argument must be an absolute path, the path must be inside your home directory, before expansion, your argument must be three characters or less.

[Key Concept]:

Every user has a home directory, typically labeled as `/home`, the home directory is where most users store their personal files. The `~` signifies the users directory, for example, `/home/user`. This means bash takes `~` and reads it as `/home/user`

[Solution]:

Since on bash startup automatically loads us into our home directory, signified by `~$` we can immediately start to invoke the command with our argument: `/challenge/run ~/h`. This will automatically create the file for us and effectively finish the challenge and the challenge will then read out the flag to terminal, thus completing it.

[# Relevant command(s) or code]:

`~` is a shortcut for the user's home directory we read `~` while Linus reads `/home/user/` for `~`

[What I Learned]:

The `~` signifies the user is in their home directory. Home directory typically stores the users personal files.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
