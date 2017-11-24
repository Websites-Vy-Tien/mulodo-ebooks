Date: 2017-11-14
Title: UNIX Tutorial Six
intro: UNIX Tutorial Six
Tags: Unix Server
Status: public
Toc: yes
Position: 7

#### Other useful UNIX commands

<code>% df .</code>: how much space is left on the fileserver

<code>% du -s *</code>: outputs the number of kilobyes used by each subdirectory. The -s flag will display only a summary (total size) and the * means all files and directories.

###### gzip

This reduces the size of a file, thus freeing valuable disk space. For example, type

<code>% ls -l science.txt</code>

and note the size of the file using ls -l . Then to compress science.txt, type

<code>% gzip science.txt</code>

This will compress the file and place it in a file called science.txt.gz

To see the change in size, type ls -l again.

To expand the file, use the gunzip command.

<code>% gunzip science.txt.gz</code>