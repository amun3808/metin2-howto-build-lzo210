# How to compile lzo

You will need to have cmake installer on your pc.
https://cmake.org/download/

1. Unzip the archive

2. Open Cmake gui

3. Where it asks `Where is the source code` put your path to the folder where you unzipped the archive

4. Where it asks `Where to build the binaries` put the same path/build

5. Click `Configure` and click "Yes" if it asks to create the folder

6. Change optional platform for generator to `Win32` and click `Finish`

7. When it's done with the configuration, click `Generate`

8. When it's done generating, click `Open Project`

9. Right click on lzo_static_lib(that's the only one you need) then go to `C/C++` -> `Code Generation` and change `Multi-threaded DLL (\MD)` to `Multi-threaded (\MT)`, then change the target to debug and change `Multi-threaded Debug DLL (\MDd)` to `Multi-threaded Debug (\MTd)`

10. Right click on lzo_static_lib -> Project Only -> Build only lzo_static_lib
