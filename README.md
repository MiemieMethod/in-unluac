unluac is a decompiler for Lua 5.0 through 5.4. It runs on Lua chunks that have been compiled with the standard Lua compiler. It requires that debugging information has not been stripped from the chunk. (By default, the Lua compiler includes this debugging information.)

This program is written in Java. A JAR package is available in the downloads section so you don't have to compile it. It runs from the command line and accepts a single argument: the file name of a Lua chunk. The decompiled code is printed to the standard output.

Here is an example usage of unluac:
java -jar unluac.jar myfile.lua > myfile_decompiled.lua

The current version also has pretty good support for Lua 5.0 and Lua 5.1. Support for later versions is also good if the code doesn't use too many gotos.
