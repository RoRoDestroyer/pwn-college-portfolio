[Position Thy Self]

Module: [Pondering Paths / Linux Luminarium]

Date: [8/31/2026]

[Objective]:

Execute the `/challenge/run` program from a specific path; must cd into that directory before running the program.

[Key Concept]:

You can navigate around in directories in Linux with the `cd` command; it stands for change directory. The path is the argument to your `cd` command. By using the `cd` command you are changing the current working directory. Each process has its own directory that it is located in. Also note that `~` means the current user's home directory.

[Solution]:

Simply execute the `/challenge/run` command to see the directory it wants you to execute the command in. Then `cd` into that directory; for me I must be in the root directory or in other words `/`. Now invoke `cd /`, now again run the `run` command from the absolute path: `/challenge/run`

[# Relevant command(s) or code]:

`cd` (change directory) is the Linux command to change the current working directory. `~` also notes the current users home directory.

[What I Learned]:

`cd` is a command that allows us to navigate Linux directories by changing our current working directory to by executing the `cd` command subsequently followed with your argument (the path of the directory you want to work in). I also learned the `~` indicates the home directory for the current user.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
