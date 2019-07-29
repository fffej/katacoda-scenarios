UNIX is an opearting system organized around the following core characteristics:

* A centrally organized kernel which manages systems and processes
* Non kernel software is organized into separate processes
* Pre-emptive multi-tasking
* A file system with a single root at `/`
* *EVERYTHING* is a file

The last point is hugely important to UNIX philosophy. Here's a philosophy for UNIX expressed by Doug Mcilroy.

* Make each program do one thing well. To do a new job, build afresh rather than complicate old programs by adding new "features".
* Expect the output of every program to become the input to another, as yet unknown, program. Don't clutter output with extraneous information. Avoid stringently columnar or binary input formats. Don't insist on interactive input.
* Design and build software, even operating systems, to be tried early, ideally within weeks. Don't hesitate to throw away the clumsy parts and rebuild them.
* Use tools in preference to unskilled help to lighten a programming task, even if you have to detour to build the tools and expect to throw some of them out after you've finished using them.

## A bit more on everything is a file.

Hard drives, modems, keyboards, printers and even network communications are just simple streams of bytes exposed through the file system.

Don't worry about the details yet. Do remember that you can use `man` and `apropos` to find out more information about a command.

A great example of this is that all system properties are available as a file. For example, here's how you could read the CPU info.

`cat /proc/cpuinfo`{{execute}}
