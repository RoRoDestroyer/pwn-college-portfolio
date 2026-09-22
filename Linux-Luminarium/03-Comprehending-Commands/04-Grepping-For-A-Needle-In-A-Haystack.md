[Grepping For A Needle In A Haystack]

Module: [Comprehending Commands / Linux Luminarium]

Date: [9/21/2026]

[Objective]:

Find the flag using the `grep` commmand on the challenge data file.

[Key Concept]:

The `grep` command works by using an argument, your specific search, and searches for that exact query for the provided file. For example, `grep test ~/test.txt` would search for the word "test" in the `~/test.txt` file.

[Solution]:

Use the `grep` command on the provided challenge file, and search for the flag (flags begin with pwn.college, so grep for that): `grep pwn.college /challenge/data.txt` 

[# Relevant command(s) or code]:

The `grep` command searches for your query in files, large or small.

[What I Learned]:

The grep command and the purpose of it. Grep is used to search files for specific data (grep SEARCH_STRING FILE). Useful when searching through large files/output.

Status: ✓ Completed on pwn.college

All work was performed within the authorized pwn.college educational environment. Challenge flags, credentials, and other restricted values are intentionally omitted.
