UNIX has a million and one commands for slicing and dicing text.

`sort` does exactly what you might expect.  Let's sort the log file in reverse.

`sort -r /var/log/dpkg.log`{{execute}}

`grep` searches for text in files. It is extremely powerful! Let's start with the basics, find all lines matching containing the exact string `status` in `/var/log/dpkg.log`

`grep status /var/log/dpkg.log`{{execute}}

We can add the `v` flag to find the lines NOT containing status.

`grep -v status /var/log/dpkg.log`{{execute}}

There's much more to learn about `grep`. Reading the manual pages is highly recommended.

One of the most powerful is `cut`. This allows you to treat each line as a delimited list and extract data appropriately. Let's extract out the first and third fields (skipping the time).

`cut -f1,3 -d" " /var/log/dpkg.log`{{execute}}

`sed` is a stream editor and can perform operations on a stream of text in a variety of ways.

TODO examples