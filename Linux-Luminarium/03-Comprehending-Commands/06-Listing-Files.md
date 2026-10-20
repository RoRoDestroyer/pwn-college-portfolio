[Listing Files]

Module: [Comprehending Commands / Linux Luminarium]

Date: [10/20/2026]

[Objective]:

List the files in `/challenge` to find '/challenge/run' for its name has been changed.

[Key Concept]:

The `ls` command is a command that lists files. If used with no arguments, just `ls` it will list the current working directory's contents. You can also use the `ls` command with arguments to list a certain directories contents without being in it, for example, `ls /example` would list `/example`'s contents.

[Solution]:

Use the `ls` command with an argument: `ls /challenge`. This will provide 2 outputs: `23656-renamed-run-18988` and `Dockerfile`, intuitively from the name we can assume that `23656-renamed-run-18988` is the correct one and we can run `/challenge/23656-renamed-run-18988` to get our flag.

[# Relevant command(s) or code]:

The `ls` command lists file contents either in the specific directory provided as an argument, or in the current working directiory if no arguments provided.

[What I Learned]:

I learned what the `ls` command is, use cases for it, and the two ways it can be utilized with and without arguments.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
