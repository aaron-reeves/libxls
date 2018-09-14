# Compiling libxls on Windows with MinGW
*A. Reeves, 14 Sep 2018*

  - sh.exe configure works as expected.
  - Makefile needs to be modified with the following line right at the top: SHELL=C:/MinGW/msys/1.0/bin/sh.exe.  This is saved in the repository as Makefile.win, but will need to be renamed for building.
  - configure.h file is not produced.  I modified a configure.h file from elsewhere, and put it in src.  This is saved in the repository as config.h.win, but needs to be renamed for building.
  -- With these changes, make works as expected.
  - Library files and executables are built, but some poking around is required to find them.


