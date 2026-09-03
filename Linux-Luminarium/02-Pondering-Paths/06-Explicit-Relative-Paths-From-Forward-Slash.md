[Explicit Relative Paths, From /]

Module: [Pondering Paths / Linux Luminarium]

Date: [9/02/2026]

[Objective]:

Your current working directory must be in the root, then the path you use to invoke `/challenge/run` must contain `.`.

[Key Concept]:

Every directory in most operating systems contains two implicit terms: `.` and `..`. The first implicit term, `.`, means to stay in the current directory you're actively in, or actively changing in. While `..` refers to going backwards, for example, `/test/challenge/..` would put us in the `/test` directory.

[Solution]:

Invoke `cd /` then invoke `/challenge/run` by the implicit relative path: `./challenge/run`

[# Relevant command(s) or code]:

`cd` changes the current working directory. There are two implicit terms: `.` and `..`. The `.` means to stay in the current working directory or the directory you're changing into via the path you're using.

[What I Learned]:

Reinforced relative paths and `cd` command. Learned the first implicit term `.`; Second implicit term, `..`, means to go backwards in the file hierarchy. 

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
