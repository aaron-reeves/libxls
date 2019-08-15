# Compiling libxls on Windows with MinGW
*A. Reeves, 14 Sep 2018*
*Updated 15 Aug 2019*

  - ```sh.exe configure``` works as expected.
  - Makefile needs to be modified with the following line right at the top: ```SHELL=C:/bin/sh.exe``` (this came from an install of Git).
  - Makefile may also need the following: ```MAKE=mingw32-make``` (replacing ```MAKE=make```).
  - ```configure.h``` file is not produced.  I modified a ```configure.h``` file from elsewhere, and put it in ```src```.  This is saved in the repository as ```config.h.win```, but needs to be renamed for building.
  -- With these changes, make works as expected.
  - Library files and executables are built, but some poking around is required to find them.


