[Position Elsewhere]

Module: [Pondering Paths / Linux Luminarium]

Date: [8/31/2026]

[Objective]:

Execute the `/challenge/run` program from a specific path; must cd into that directory before running the command, must do this five different times, in five different paths.

[Key Concept]:

You can navigate around in directories in Linux with the `cd` command. The path following the `cd` command is considered the argument to the command. Requesting to change into a directory that starts at the root `/` is considered the absolute path.

[Solution]:

Simply execute the `/challenge/run` command to see the directory it wants you to execute the command in. Then `cd` into that directory; for me I must be in `/var/lib/apt/lists`. Now invoke `cd /var/lib/apt/lists`, now again run the `run` command from the absolute path: `/challenge/run`; in the new directory. Now we will get level 2, `/tmp` is now the requested directory, invoke cd `/tmp`, now once again execute the `run` command from the absolute path: `/challenge/run`. Now the requested directory is `/sys`, execute `cd /sys`, then run `/challenge/run`. Once again a new directory is requested, we must `cd` into `/usr/bin`: `cd /usr/bin`, now execute `/challenge/run` again. Lastly for level 5, we are now requested to change into the `/etc` directory, lastly we will execute `cd /etc` and run `/challenge/run` and at last we will get our well earned flag.

[# Relevant command(s) or code]:

`cd` (change directory) is the Linux command to change the current working directory. Any command being executed that starts at the root `/` is considered being executed by the absolute path.

[What I Learned]:

Using the command `cd` allows us to navigate Linux directories by passing arguments into it, also known as our path. Once we type `cd` we subsequently follow it by our path (argument), which allows us to change our current working directory. Any command being executed that starts with `/` is being executed by the absolute path.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
