# Internal memory scanning

This is just for learning purposes.

The goal is to have a value scan similar to cheat engine

then maybe use it to create patterns ?

that would be pog

## Current state :
the scan works if you know the average memory region of the value,

The problem being that idk where a program values are, they are not close to the program's module base

they seem to be randomized each time i run the dummy program, unlike the program's module addr which seems to be static


Notes

VirtualQuery could be usefull to scan a lot of the memory without triggering STATUS_ACCESS_VIOLATION, maybe ?
addr % page len gives us the current page index. right ?

https://github.com/darfink/region-rs this could be a good learning source 