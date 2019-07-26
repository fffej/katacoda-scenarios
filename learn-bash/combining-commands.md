The real power of UNIX systems comes from combining. The underlying philosophy of UNIX is that power comes from combining things together.

Let's look at a number of ways we can do that.

The `|` operator feeds the output of the left hand side into the input of the right hand side. For example, the following sorts the output of listing the root directory backwards.

`ls / | sort -r`{{execute}}

You can append any number of pipe operators into to create commands. Let's find out what the most common starting letter of directory names is. This introduces a few new commands. Use `man` to find out what they do!

`ls / | cut -c1 | sort -rn | uniq -c | sort -rn`{{execute}}

`tr` is a textual replacement command. Let's use that to translate the `ls /` command to be more shouty by textually replacing all lowerclass characters with their upper class equivalents (as always, use `man tr` to find out more information).

`ls -al | tr [:lower:] [:upper:]`{{execute}}

The `sed` command is a powerful stream editor for filtering and transforming text. Perhaps the most common use of this is to perform regular expression search and replace.

`ls -al | sed s/root/ROOT/g`{{execute}}