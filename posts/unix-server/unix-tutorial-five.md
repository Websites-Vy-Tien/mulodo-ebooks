Date: 2017-11-14
Title: UNIX Tutorial Five
intro: UNIX Tutorial Five
Tags: Unix Server
Status: public
Toc: yes
Position: 6

#### File system security (access rights)

In your <b>unixstuff</b> directory, type

<code>% ls -l</code>

![](http://www.ee.surrey.ac.uk/Teaching/Unix/file1.gif)

The 9 remaining symbols indicate the permissions, or access rights, and are taken as three groups of 3. 


+ The left group of 3 gives the file permissions for the user that owns the file (or directory) (ee51ab in the above example);
+ the middle group gives the permissions for the group of people to whom the file (or directory) belongs (eebeng95 in the above example);
+ the rightmost group gives the permissions for all others.

###### Access rights on files.

+ r (or -), indicates read permission (or otherwise), that is, the presence or absence of permission to read and copy the file
+ w (or -), indicates write permission (or otherwise), that is, the permission (or otherwise) to change a file
+ x (or -), indicates execution permission (or otherwise), that is, the permission to execute a file, where appropriate

###### Access rights on directories.


+ r allows users to list files in the directory;
+ w means that users may delete files from the directory or move files into it;
+ x means the right to access files in the directory. This implies that you may read files in the directory provided you have read permission on the individual files.

#### Changing access rights

###### chmod (changing a file mode)

Only the owner of a file can use chmod to change the permissions of a file. The options of chmod are as follows

<table cellspacing="0" cellpadding="3" bordercolor="#666666" border="1" align="center">
  <tbody><tr> 
    <th>Symbol</th>
    <th>Meaning</th>
  </tr>
  <tr> 
    <td><div align="center">u</div></td>
    <td>user</td>
  </tr>
  <tr> 
    <td><div align="center">g</div></td>
    <td>group</td>
  </tr>
  <tr> 
    <td><div align="center">o</div></td>
    <td>other</td>
  </tr>
  <tr> 
    <td><div align="center">a</div></td>
    <td>all</td>
  </tr>
  <tr> 
    <td><div align="center">r</div></td>
    <td>read</td>
  </tr>
  <tr> 
    <td><div align="center">w</div></td>
    <td>write (and delete)</td>
  </tr>
  <tr> 
    <td><div align="center">x</div></td>
    <td>execute (and access directory) </td>
  </tr>
  <tr> 
    <td><div align="center">+</div></td>
    <td>add permission</td>
  </tr>
  <tr> 
    <td><div align="center">-</div></td>
    <td>take away permission</td>
  </tr>
</tbody></table>

For example, to remove read write and execute permissions on the file <b>biglist</b> for the group and others, type

<code>% chmod go-rwx biglist</code>: This will leave the other permissions unaffected.

To give read and write permissions on the file <b>biglist</b> to all,

<code>% chmod a+rw biglist</code>

