# Persistence

Persistence is important in almost any case of a trojan horse if you want to do more damage.
In most operating systems, there is a standard folder in which you can include files to be run on startup, using
these folders is bad practice and should be avoided.

## Notes

This guide will **not** help you if you are writing for (linux, android, etc) and is recommended only for use in Windows cases.
This guide will also not try to spoonfeed you information but rather help you in your journey to becoming a malware master!

## The overwriting of files

Overwriting files is one way to gain persistence on a poorly protected machine. Some anti-viruses may not even know you have
overwritten a file. 

In order to make the process believable in most use cases, read the original file, move it to a hidden location, write a new file
that will run the original file whilst also running your payload, a watchdog is recommended to stop user tampering.

## The modification of files

Writing new data to files that are run at program startup is another way to maintain access, for example, in a manifest
file that contains a list of files to run, include the path to your malware executable hidden in a folder out of
sight, simple, right?
