[Implicit Relative Path]

Module: [Pondering Paths / Linux Luminarium]

Date: [9/02/2026]

[Objective]:

Execute the `/challenge/run` command while in the `/challenge` directory.

[Key Concept]:

The implicit term `.` refers to staying in the same directory that you're currently in or actively changing into. When running commands if you're in the directory right before the command, for example, `test/command` is where our command lives but were in the `/test` directory, simply typing `command` will result in a bash error. This is because linux safety nets this due to the possibility a command were to have the same name as a system utility. This is because if there were identical names, the system utility would be executed instead rather than our command. 

[Solution]:

`cd` into `/challenge` then invoke the `/challenge/run` command via the explicit path: `./run`.

[# Relevant command(s) or code]:

`cd` changes directories. The implicit term `.` refers to stay in the current directory.

[What I Learned]:

Why linux commands don't run at the bare name when in the prior directory; relative to file hierarchy. Reinforced using implicit terms and proper use cases. 

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
