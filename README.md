tswav
=====

Command line tool to transform a stereophonic sound (2 channels) WAVE file.

License
-------

zlib License.

Target environments
-------------------

Windows, Cygwin, Linux, macOS.

tswav is Python 2.7 script, and so probably works fine on other OS.

Set up
------

1. Install Python 2.7.13 or later.
2. Put tswav in a directory registered in PATH.

Usage
-----

Please check help message `tswav --help`

Example
-------

```sh
# In the following cases, output.wav has 2 channels pcm data.

# stereo to mono (mix left/right channels: default behavior)
tswav -o output.wav input.wav
tswav -t mix -o output.wav input.wav

# pick up left channel
tswav -t left -o output.wav input.wav

# pick up right channel
tswav -t right -o output.wav input.wav

# swap left/right channels
tswav -t swap -o output.wav input.wav
```
