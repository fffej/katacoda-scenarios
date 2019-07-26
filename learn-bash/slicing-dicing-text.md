UNIX has a million and one commands for slicing and dicing text.

One of the most powerful is `cut`. This allows you to treat each line as a delimited list and extract data appropriately. Let's extract out the first and third fields (skipping the time).

`cut -f1,3 -d" " /var/log/dpkg.log`{{execute}}

Similarly, `sort` does exactly what you might expect.  Let's sort the log file in reverse.

`sort -r /var/log/dpkg.log`{{execute}}