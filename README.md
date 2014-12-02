# Perception

Perception is a hobby operating system. There are multiple components to this project. Shovel is a programming language being developed for Perception.

Shovel and Turkey are being developed seperately from Perception, so that they may be embedded into any system or application.


## Running
Either build the operating system from source or download a prebuilt image (comming soon) and boot it. Use the Windows key to access the shell that
allows you to launch applications.

To set a custom resolution, press 'E' in GRUB, and replace the 'auto' on "set gfxpayload=auto" with a resolution (in the format of WidthxHeightxBPP or WidthxHeight) and press F10 to boot.

## Features:
Some of the features of the operating system are:
- A shell that discovers programs on mounted disks and manages running processes (press the Windows key to access it at any time).
- Asynchronous/event-based programming API.
- ISO 9660 read support.
- Composting tabbing window manager with full-screen dithering (press F10 in non-24 bit colour modes to toggle dithering).
- VBE video and a fall back VGA driver.


## Directory Structure
- Applications - The sources for the applications that come with Perception.
- build - Tools for cross-compiling the applications and libraries.
- fs - The root file system that is turned into a disk image.
- kernel - The kernel sources.
- Libraries - The sources of libraries that run under Perception.
- shovel - Tools related to the Shovel language build system - compiler, assembler
- turkey - Turkey is a virtual machine that runs Shovel programs.


## Todo
This is a very high level to-do list. Near term goals of Perception include:
- Loading programs.
- RAM disk.
- Some nice sample programs (Calculator, Text Editor, File Manager, Minesweeper).

Eventual goals:
- Build a terminal emulator built around Shovel.
- Port the build tools to run under Perception.
- Build an IDE in Perception.

Long term goals:
- Make a great OS.

Near term goals of Shovel include:
- Optimize SSA (constant propagation, deadcode elimination).
- Implement basic block versioning JIT.
- Change C API to work with JIT.

## Want to help?
I would be interested in accepting patches, mainly those that improve performance (such as new optimizations for Turkey) or clean up
code (the SSA generator is really messy!)

Contains DejaVu fonts: http://dejavu-fonts.org
