One area that UNIX excels at is text manipulation.

To start things off, let's look at a big file. The `cat` command displays a file as text. Let's have a look at a log file.

`cat ~/countries.txt`{{execute}}

Hopefully you just saw some text whiz by. That's a bit annoying though, since really you want to be able to read it. You can use the `more` command to paginate output. Handy tip! Press `q` to quit.

`more ~/countries.txt`{{execute}}

But what's better than `more`? The answer is of course `less`.

`less ~/countries.txt`{{execute}}

To get an idea of the difference between the two, you can use `man more` or `man less` to find out the nitty gritty details.

What if you just want to look at the first few lines?

`head ~/countries.txt`{{execute}}

Or the last?

`tail ~/countries.txt`{{execute}}