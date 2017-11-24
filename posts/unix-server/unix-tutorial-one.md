Date: 2017-11-14
Title: UNIX Tutorial One
intro: UNIX Tutorial One
Tags: Unix Server
Status: public
Toc: yes
Position: 2

#### Listing files and directories

###### To find out what is in your home directory, type

<code> % ls </code>

###### To list all files in your home directory including those whose names begin with a dot, type 

<code>% ls -a</code>

###### To list all files in your define folder

<code>% ls [your folder path]</code>

Examples:

<code>% ls myFolder</code>
<code>% ls myFolder/mySubFolder</code>

###### Home directories can also be referred to by the tilde ~ character. It can be used to specify paths starting at your home directory. So typing

<code> % ls ~/[your folder name]</code>

Example:

<code>% ls ~/documents</code>

It will be shown all files of folder: <code>/Users/mac-l011/documents</code>

###### List all files in the file system

<code> % ls ~</code>

###### List all files in the parent's file system

<code> % ls ~/..</code>

#### Making Directories

###### To create sub folder from current folder

<code>% mkdir [your folder name]</code>

Example:

<code>% mkdir myNewFolder</code>

#### Changing to a different directory

###### To change to the directory, type

<code>% cd [your folder path]</code>

###### To change to the parent directory, type

<code>% cd ..</code>

#### Pathnames

###### To find out the absolute pathname of your home-directory

<code>% pwd</code>