# Lua API

This page documents the Lua API, as implemented in this libary

## General

`print(string)`: Print text to the web output.

`println(string)`: Print text to the web output and add a newline.


## Loading Files

`include(filename)`: Include a file that may include `<?lua` sections.
The same file may be included multiple times using this method.

`dofile(filename)`: Include and execute a file that contains _only_ Lua
code. `<?lua` is not required or supported in these files.

## Logging

The `log` module contains the following methods:

- `info(msg, [param...])`: Log an informational message.
- `debug(msg, [param...])`: Log a debug message.
- `warn(msg, [param...])`: Log a warning message.
- `error(msg, [param...])`: Log an error message.
