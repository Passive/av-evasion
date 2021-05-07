# Evading analysis

Evading analysis is not necessary if you are writing a quick virus just for fun, but if you
want to stay undetected and otherwise "safe" you must atleast attempt to avoid detection
by analysis

## Techniques

When it comes to analysis, most people think of "AI" or artificial intelligence. Believe it
or not, manual analysis exists. Some people will try to see what your virus touches, how
it moves, what functions it uses and what they do.

After running a program some people like to try to open the executable in IDA or "The interactive disassembler". If you
obfuscate your code you should have no issues with things like this, you can also create an external watchdog to check
on your virus.

Try to detect virtual machines, you can find some good tutorials online showcasing
just how to do this (https://stackoverflow.com/questions/41750144/c-how-to-detect-the-virtual-machine-your-application-is-running-in-has-focus)

You can also follow some basic tips such as taking your time, making sure to regularly check if the user is
trying anything, etc.

### I hope you enjoyed this short guide..
