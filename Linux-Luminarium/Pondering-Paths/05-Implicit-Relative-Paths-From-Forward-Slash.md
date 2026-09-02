[Implicit Relative Paths From, /]

Module: [Pondering Paths / Linux Luminarium]

Date: [9/02/2026]

[Objective]:

Change your current working directory to the root, `/`; then invoke `/challenge/run` by its relative path.

[Key Concept]:

When using absolute paths, it does not matter what directory you're in. A relative path is any path that does not start at the root, `/`; a relative path is relative to your current working directory (cwd). Your cwd is the current directory you're actively working in. 

[Solution]:

Use the `cd` command to change your directory to the root: `cd /`. Then invoke the `/challenge/run` from the relative path: `challenge/run`.

[# Relevant command(s) or code]:

`cd` changes the current working directory and the relative path is relative to the current directory you're in, for example, if we have a command at `/GitHub/test/command` if we are in the directory: `/GitHub`. Then we only need to execute the command by invoking `test/command`, or if in the directory: `/GitHub/test`. Then we can invoke the command by writing `command`.

[What I Learned]:

The difference between relative and absolute paths; what a relative path actually relates to. Reinforced changing directories.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
