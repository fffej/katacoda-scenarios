Unix has plenty of options for editing text.

Regardless of what you choose, always understand enough `vi` to be able to edit text, as it's available on almost all systems. `emacs` is a good choice too, and is especially awesome when customized.

# ed

The original editor was known as `ed`. `ed` is a line oriented editor and it's available everywhere. It's also been described as _the most user-hostile editor ever created_ ([Peter Salus](https://en.wikipedia.org/wiki/Peter_H._Salus)).

Let's create a hello world in ed. 

`ed`{{execute}}

At startup, `ed` is in command mode. Let's type `a` (and press return) to get it into append-mode. Now type the text you want on a single line (e.g. `Hello world!`) and press return. Now this is a single line in the buffer. Type `.` and press return to exit append mode. Now you are at a command prompt again, type `w ~/helloworld.txt`, press return and press `q` and return to exit.

Now take a deep breath and hope that

`cat ~/helloworld.txt`{{execute}}

Displays the text you entered.

# vi

`vi` builds upon `ed` and is considered _sligthly_ friendlier.

![Exiting Vim](https://github.com/fffej/katacoda-scenarios/raw/master/learn-bash/images/exiting-vim.jpg)

The main thing to realize is that `vi` has both a command mode and an insert mode. 

`vi hello.txt`{{execute}}

Switch to command mode by pressing `Esc`.

To exit `vi`, then `Esc` to get into command mode and type `q!` to exit without changes.

# emacs

Emacs is an extensible ~operating system~ text editor written in Lisp. It can be heavily customized to do more or less anything. It's not installed by default on most systems.

It's not installed by default on most systems (but you can install it with `sudo apt-get update && sudo apt-get install -y emacs` in the terminal if you want to experiment).






