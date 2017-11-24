Date: 2017-11-14
Title: UNIX Tutorial Three
intro: UNIX Tutorial Three
Tags: Unix Server
Status: public
Toc: yes
Position: 4

#### Redirecting/Writting the Output

We use the <b> > </b> symbol to redirect/write the output of a command.

<code>% cat >[filename]</code>

Then press content that you want to write and press <b>Ctrl + C/D</b> to exit

To read the contents of the file, type

<code>% cat [filename]</code>

#### Appending to a file

The form <b> >> </b> appends standard output to a file. So to add more items to the file, type

<code>% cat >>[filename]</code>

Use the <b>cat</b> command to join (concatenate) <b>filename1</b> and <b>filename2</b> into a new file called <b>filename3</b> or overwrite content for existed file <b>filename3</b>. Type

<code>cat [filename1] [filename2] > [filename3]</code>

#### Pipes

To see who is on the system with you, type

<code>% who</code>

One method to get a sorted list of names is to type,

<code>% who > names.txt</code>
<code>% sort < names.txt</code>

It will write a sorted list of names into file <b>names.txt</b>