
# File permissions in Linux

## Project description

![](data:image/png;base64...)

## Check file and directory details

This document displays the file structure of the /home/researcher2/projects directory and the permissions of the files and subdirectory it contains.

In the /home/researcher2/projects directory, there are five files with the following names and permissions:

* project\_k.txt
  + User = read, write,
  + Group = read, write
  + Other = read, write
* project\_m.txt
  + User = read, write
  + Group = read
  + Other = none
* project\_r.txt
  + User= read, write
  + Group = read, write
  + Other = read
* project\_t.txt
  + User = read, write
  + Group = read, write
  + Other = read
* .project\_x.txt
  + User = read, write
  + Group = write
  + Other = none

There is also one subdirectory inside the projects directory named drafts. The permissions on drafts are:

* User = read, write, execute
* Group = execute
* Other = none

## Describe the permissions string

![A screen shot of a computer

Description automatically generated with medium confidence](data:image/png;base64...)

* For this example we are going to use the project\_k.txt doc for our string explanation
* So for this doc we have “-rw-rw-rw-“ the first character stands for either directory (d) or file (-), the next 3 strings describe the access that each member is allowed to the directory or file: User, Group, Other.
* Also as well we have four different meanings for access to these groups which falls as: (-) none, (r) read, (w) write, & (x) execute.
* So finally our string will read as project\_k.txt file is enabled access to User: read & write, Group: read & write, & Other: read and write

## Change file permissions

![A picture containing graphical user interface

Description automatically generated](data:image/png;base64...)

* Say still using the example for file project\_k we wish to change the access of others to absolutely none to secure this file this is how we would do this.
* As you see: you use chmod (change mode) and then follow up with who’s access you wish to change followed by either signage of (-) remove or, (+) add permission then follow up lastly with which are you are specifying.

## Change file permissions on a hidden file

![Text

Description automatically generated with medium confidence](data:image/png;base64...)

* In this snipped we are changing permissions to a hidden file. It is the same concept as a file that is not hidden except we use the command (ls) list, then (-la) hidden permissions to achieve this task.

## Change directory permissions

![Graphical user interface

Description automatically generated with medium confidence](data:image/png;base64...)

* Finally we are wanting to remove the executable privileges from the group from our drafts directory. To achieve this we make sure that we are in the parent directory as you cannot change the permissions of a subdirectory while in it, then we go about our normal route of changing permissions.

## Summary

In summary this is how you will go into Linux’s GLI and navigate, change directories, explore permissions, and even change permissions not only for files but for entire directories as well. This is extremely helpful as a security analyst as making sure that your companies infrastructure is always key to cybersecurity and preventing an attack.

