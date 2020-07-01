# findRelevant
Python program designed for `Makefile`s. I built this because `$(find)` and all of its parameters got a little confusing.
Run `./findRelevant.py -h` to display the help menu:

Usage:	`./findRelevant.py -flag <extension> (exclusions)`

Flags:
* `-help` or `-h` displays options,
* `-f` returns only filenames with no extension,
* `-o` returns filenames with '.o' appended,
* `-x` returns filenames with '.exe' appended, and 
* `-e` returns filenames with extensions kept.
* `<extension>` designates the extension to search for, and
* `(exclusions)` are files to be excluded from output.

For example, in a directory containing `file1.cpp file2.cpp file3.cpp file4.cpp file5.cpp`, 

`./findRelevant.py -f .cpp file3.cpp file4.cpp` would output 

`file1 file2 file5`.
