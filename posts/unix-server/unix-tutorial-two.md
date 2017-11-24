Date: 2017-11-14
Title: UNIX Tutorial Two
intro: UNIX Tutorial Two
Tags: Unix Server
Status: public
Toc: yes
Position: 3

#### Copying Files

###### To make a copy of file1 in the current working directory and calls it file2

<code>% cp file1 file2</code>

###### To make a copy of file1 in other folder to current folder with the same name

<code>% cp [file 1 folder]/file1 .</code>

Example:

<code> % cp /vol/ee/ee-info/Teaching/Unix/science.txt .</code>

#### Moving files

###### To move (or rename) file1 to file2

<code>% mv file1 file2</code>

+ To move a file from one place to another, use the mv command. This has the effect of moving rather than copying the file, so you end up with only one file rather than two.
+ It can also be used to rename a file, by moving the file to the same directory, but giving it a different name. 

Example:

<code> % mv science.bak backups/.</code>

Move file science.bak to folder backups with same name

#### Removing files and directories

###### To remove file or directories, type

<code>% rm (remove)</code>
<code>% rmdir (remove directory)</code>

#### Displaying the contents of a file on the screen

###### To display the contents of a file on the screen. Type:

<code>% cat [filename]</code>

###### The command less writes the contents of a file onto the screen a page at a time. Type

<code>% less [filename]</code>

After that, existing this process: <code>: q</code>

###### The head command writes the first ten lines of a file to the screen.

<code>% head [number lines (optional)] [filename]</code>

###### The tail command writes the last ten lines of a file to the screen. 

<code>% tail [number lines (optional)] [filename]</code>

#### Searching the contents of a file

###### Simple searching using less

Using <b>less</b>, you can search though a text file for a keyword (pattern). For example, to search through science.txt for the word 'science', type 

<code>% less science.txt</code>

then, still in <b>less</b>, type a forward slash <b>[/]</b> followed by the word to search

<code>/science</code>

###### grep

It searches files for specified words or patterns.

<code>% grep [keyword] [filename]</code>

The grep command is case sensitive; To ignore upper/lower case distinctions, use the -i option, i.e. type 

<code>% grep -i [keyword] [filename]</code>

Example:

<code> % grep -i 'spinning top' science.txt</code>

Some of the other options of grep are:
- <code>-v</code> display those lines that do NOT match
- <code>-n</code> precede each matching line with the line number
- <code>-c</code> print only the total count of matched lines 

###### wc (word count)

A handy little utility is the wc command, short for word count. To do a word count on science.txt, type

<code>% wc -w [filename]</code>

To find out how many lines the file has, type

<code>% wc -l [filename]</code>

#### Other command lines

###### To clear the terminal window of the previous commands so the output of the following commands can be clearly understood

<code>% clear</code>
