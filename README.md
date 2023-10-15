# Ring_Text_Gimp_Plugin
Make Ring Text in Gimp using this Plugin. Below is two image previews of this plugin with two different aesthetics

![image](https://github.com/LinuxBeaver/Ring_Text_Gimp_Plugin/assets/78667207/b6bc5a59-914a-429a-9796-595a31bbcb8c)
![image](https://github.com/LinuxBeaver/Ring_Text_Gimp_Plugin/assets/78667207/3f48dbb2-d0d0-4914-a31e-f56a3d99c718)


Download binaries here. (FOLLOW INSTRUCTIONS)
https://github.com/LinuxBeaver/Gimp_Ring_Text/releases


## OS specific location to put GEGL Filter binaries 

**Windows**
C:\Users\USERNAME\AppData\Local\gegl-0.4\plug-ins
 
** Linux **
 /home/(USERNAME)/.local/share/gegl-0.4/plug-ins
 
 **Linux (Flatpak)**
 /home/(USERNAME)/.var/app/org.gimp.GIMP/data/gegl-0.4/plug-ins

![image](https://github.com/LinuxBeaver/GEGL-glossy-balloon-text-styling/assets/78667207/f15fb5eb-c8d7-4c08-bbac-97048864e657)


## Compiling and Installing
**Linux**

To compile and install you will need the GEGL header files (libgegl-dev on Debian based distributions or gegl on Arch Linux) and meson (meson on most distributions).

meson setup --buildtype=release build
ninja -C build


If you have an older version of gegl you may need to copy to ~/.local/share/gegl-0.3/plug-ins instead (on Ubuntu 18.04 for example).

**Windows**

The easiest way to compile this project on Windows is by using msys2. Download and install it from here: https://www.msys2.org/

Open a msys2 terminal with C:\msys64\mingw64.exe. Run the following to install required build dependencies:

pacman --noconfirm -S base-devel mingw-w64-x86_64-toolchain mingw-w64-x86_64-meson mingw-w64-x86_64-gegl

Then build the same way you would on Linux:

meson setup --buildtype=release build
ninja -C build

## Preview of this plugin using its "gegl syntax mode" correctly. the syntax makes the fancy effect.

![image](https://github.com/LinuxBeaver/GEGL-glossy-balloon-text-styling/assets/78667207/b23303be-edeb-4b4d-9015-0209dab12689)

![image](https://github.com/LinuxBeaver/Ring_Text_Gimp_Plugin/assets/78667207/ba1e9b7e-969d-4d1a-b9e2-b54181a698c1)


