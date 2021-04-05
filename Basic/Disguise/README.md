# Disguising your virus
Disguising your virus can be challenging depending on what it does, if it goes around doing random calls, adding regkeys
and copying itself, yeaaaaaah no. But if your virus is built to hide itself, you should be fine.

## WinAPI calls
Try to avoid using the windows API, it can be a dead giveaway!

## System calls
Instead of attempting to run your commands using the `system` method, try finding a less obvious
way of executing your code.

## String contents / method names
Some antiviruses will attempt to disassemble your executable and check the method names and string contents,
make sure to keep it clean in there!

## Do not do everything at once
This is an obvious one, but yes, do not go around deleting files and then creating copies of yourself!!1!!!!1
