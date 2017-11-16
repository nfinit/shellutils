# Shell utilities
A collection of independent shell scripts targeted at legacy Unix systems.

This repository exists to accumulate small shell scripts of use for users of legacy or otherwise esoteric operating systems with limited software availability or other handicaps which require creative (or just kludgy) usage of basic utilities to accomplish certain tasks, such as taking screenshots.

### Contents
There's currently only a single script in this repository:
* `capture`: An extremely crude full-screen capture tool written for use on an HP-UX 11i system for which a working build of ImageMagick was unavailable. `capture` takes a screenshot using `xwd -root` and sends the file to another system to convert to a PNG or other user-specified format using ImageMagick on a remote system. `capture` connects to the remote host purely through SSH and SCP to maximize compatibility, with a trade-off of requiring you to enter your password for every stage of the process.
