Date: 2017-11-14
Title: UNIX Tutorial Four
intro: UNIX Tutorial Four
Tags: Unix Server
Status: public
Toc: yes
Position: 5

#### Wildcards

###### The * wildcard

The character * is called a wildcard, and will match against none or more character(s) in a file (or directory) name. For example, in your <b>unixstuff</b>b> directory, type

<code>% ls list*</code>: This will list all files in the current directory starting with <b>list....</b>

<code>% ls *list</code>: This will list all files in the current directory ending with <b>....list</b>

###### The ? wildcard 

The character <b>?</b> will match exactly one character.
So <b>?ouse</b> will match files like <b>house and mouse, but not grouse.</b>
Try typing

<code> % ls ?ouse</code>

#### Filename conventions

We should note here that a directory is merely a special type of file. So the rules and conventions for naming files apply also to directories.

In naming files, characters with special meanings such as / * & % , should be avoided. Also, avoid using spaces within names. The safest way to name a file is to use only alphanumeric characters, that is, letters and numbers, together with _ (underscore) and . (dot).

| Good filenames   |      Bad filenames       |
|------------------|--------------------------|
| project.txt      |  project                 |
| my_big_program.c |  my big program.c        |
| fred_dave.doc    |  fred & dave.doc         |