# Linux Permissions

Each file has some properties associated with it.

Let's explore those by listing all files in `/usr/bin/` that begin with an `x`.

`ls /usr/bin/x*`{{execute}}

You'll notice a bunch of files are listed. Let's examine what each column means:

The first column looks somewhat like `-rwxr-xr-x`. Let's break this down. The first character is either `-`, `d` or `l` which mean file, directory or link. The remaining 9 characters correspond to permissions for owner, group and other users. Each three characters corresponds to permissions to read/write/execute. In our example, `-rwxr-xr-x` is a file. The owner can (r)ead w(rite) and e(x)ecute the file. The group owning the file is similar but cannot (w)rite. Similarly, other uses can only (r)ead and e(x)ecute.


