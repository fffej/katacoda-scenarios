# Linux File Permissions

Each file has some properties associated with it.

Let's explore those by listing all files in `/usr/bin/` that begin with an `x`.

`ls -al /usr/bin/x*`{{execute}}

You'll notice a bunch of files are listed. Let's examine what each column means:

The first column looks somewhat like `-rwxr-xr-x`. Let's break this down. 

The first character is either `-`, `d` or `l` which mean file, directory or link. The remaining 9 characters correspond to permissions for owner, group and other users. 

Each group of three characters corresponds to permissions to read/write/execute. In our example, `-rwxr-xr-x` is a file. The owner can (r)ead (w)rite and e(x)ecute the file. The group owning the file is similar but cannot (w)rite. Similarly, other uses can only (r)ead and e(x)ecute.

After the permissions, comes a number. This represents the number of files inside the directory (or 1 if it's just a file). Next up are the owner(e.g. `root`) and group (e.g. `root`). Next up is the size of the file in bytes, the date of last modification and finally, the name of the file.


