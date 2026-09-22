[Comparing Files]

Module: [Comprehending Commands / Linux Luminarium]

Date: [9/22/2026]

[Objective]:

There are two files: `/challenge/decoys_only.txt` contains 100 fake flags and `/challenge/decoys_and_real.txt` contains all 100 fake flags, plus the one real flag. Using the difference command, find the real flag.

[Key Concept]:

The `diff` command compares two files line by line to find the differences in each file. Upon finding the difference, alongside the textual difference it will provide the specific line that changed. For example if we have two files that are nearly the same but line 3 is different. The `diff` command will show us that difference with `2a3` which means after line 2 of file one, add line 3.

[Solution]:

To find the real flag, compare the difference of the files with our `diff` command (diff FILE_1 FILE_2): `diff /challenge/decoys_only.txt /challenge/decoys_and_real.txt`. Also note the output before the flag for this specific challenge will note `78a79` to further establish the meaning of this, this specific example means after line 78 in file 1, add line 79 of file 2.

[# Relevant command(s) or code]:

The `diff` command is good at finding differences in files, unlike `grep` instead of searching for a specific content in a file, we can search for the differences between two files, which could be unknown, and for `grep` that specific content would have to be known.

[What I Learned]:

The purpose of the `diff` command, general use case for it. Also learned the output structure that `diff` provides, that lets us know what lines changed in a file.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
