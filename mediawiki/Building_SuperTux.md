[[Template:Milestone 2]]  [[Template:Outdated]]
'''Outdated''': SVN version uses cmake/make instead of autoconf/jam. See [http://supertux.lethargik.org/viewvc/viewvc.cgi/trunk/supertux/INSTALL?view=markup INSTALL]. 

= Some notes for windows users =

Supertux development mainly happens on Linux. The source code is written in a portable manner but the tools and development environment for windows isn't there. However, you should be able to get the game built with the help of MSYS and MinGW. Find more detailed instructions at [[Building on Windows]].

You can also cross-compile the game with MinGW or [[Cross_compiling_with_MXE|M Cross Environment]].

Prebuilt binaries can be found at [[User:Rgcjonas]]

= Mac OS X =

[[User:RavuAlHemio|Ravu al Hemio]] has written a [[User:RavuAlHemio/Mac_OS_X_compilation|guide]] for Mac OS X Tiger users on building SuperTux <=0.3.1.

[[User:x2on|x2on]] writes a [[User:x2on/Mac_OS_X_compilation|guide]] for Mac OS X Snow Leopard users on building SuperTux >=0.3.2 SVN.

A new guide for building SuperTux >= 0.3.3 Git is [http://www.x2on.de/2012/01/28/tutorial-building-supertux-0-3-3-on-mac-os-x-lion/ here] available

= Prerequisites =

You will need the following tools and libraries to build SuperTux on your system:
* gcc compiler &co (gcc, g++, binutils, glibc)
* gettext
* autoconf
* cmake
* SDL (*)
* SDL-image (*)
* PhysFS (*)
* Ogg/Vorbis (*)
* OpenGL (*)
* OpenAL (*)
* libcurl (*) (optional)
* libboost (*) (SVN only)
* libglew (*) (SVN only)

You should make sure that you also have development headers and libraries installed for the tools marked with (*).

Most distributions offer separate developer versions for these libraries.

== Debian ==
Debian users should run
 apt-get install subversion autoconf automake jam g++ 
 apt-get install libsdl1.2-dev libsdl-image1.2-dev libphysfs-dev libvorbis-dev libogg-dev libopenal-dev
and (if you want the Add-on Manager)
 apt-get install libcurl3-dev
to install them.

== Ubuntu ==
  Tested on Ubuntu 14.04 (Trusty Tahr), but probably the process works in other versions of system.
  The way is very simple, but I have detailed here to facilitate the process. 
  Follow the steps below:

First of all, set the "sources" of Ubuntu:

Open the [[Software and Updates]] and [[Ubuntu Software]] tab select [[Main Server]] in the [[Download from]]; in the [[Other Software]] tab check the two [[Independent]] boxes. Click [[Close]] and then [[Reload]]. Wait for the update process to finish. 
----


1. Open the Terminal and use the "[[sudo apt-get build-dep supertux]]" command and after use "[[s]]" to confirm;

2. Use the following commands, one after the other, and wait to download them:
   sudo apt-get install libsdl2-2.0-0
   sudo apt-get install libsdl2-dev
   sudo apt-get install libsdl2-image-2.0-0
   sudo apt-get install libsdl2-image-dev

3. Using Mozilla Firefox or the browser you prefer, download this file:
   [http://ftp.gnu.org/gnu/libiconv/libiconv-1.12.tar.gz libiconv 1.12]
...and unzip it in the ''Home'' folder. In Terminal, use the following commands:
   cd /home/user/libiconv-1.12 (replace the [[user]] name of your account user)
   ./configure --prefix=/usr
   sudo make
   sudo make install

4. [https://code.google.com/p/supertux/source/browse/ Open this link and click on "Download .zip"]
After downloading, unzip the downloaded file to the [[Home]] folder and rename it to ''"supertux"'' (without quotes).

5. In Terminal, use these commands:
   cd/home/user/supertux (replace the [[user]] name of your account User)
   mkdir build
   cd build
   cmake -DDEBUG=ON ..
   sudo make (this is a long process)
   sudo make install

Just go in ''supertux'' folder you will find the game compiled and ready to run.

== Gentoo ==
Gentoo users should run
 emerge -avn subversion ftjam media-libs/openal physfs libsdl sdl-image libvorbis libogg
and (if you want the Add-on Manager)
 emerge -avn curl

== FC6 ==
For Fedora, use <code>yum</code> and don't forget the development packages!
 yum install jam SDL SDL-devel SDL_image SDL_image-devel physfs physfs-devel openal openal-devel
(assuming gcc, gettext and autoconf are already installed)

= Source Code from release ≤ 0.3.1 =
== Configuring the source ==

Before compiling the source code you have to configure it so that it gets adapted to your machine. Use the following commands:

 ./autogen.sh
 ./configure --enable-debug

configure checks if all prerequisites are met.

== Compiling the source ==

You can compile the source code from commandline with the help of jam. Simply type

 jam

and the game should build. You should [[SuperTux FAQ#How can I get in touch with you.3F|Contact]] us in case of errors or problems.

= Source Code from release ≥ 0.3.1 and from SVN =
== Getting the source from SVN ==

The first thing to get started with supertux is getting the latest development resources from the subversion repository. How to do this is described here at [[Download/Subversion]].

== Configuring and Compiling ==

SuperTux uses CMake to generate a set of Makefiles for the build process. To generate these Makefiles and build SuperTux, perform the following steps which are also described in [http://supertux.lethargik.org/viewvc/viewvc.cgi/trunk/supertux/INSTALL?view=markup INSTALL]
which comes in the source archive.

# `cd' to the directory where you unpacked the SuperTux source archive, i.e. to the directory containing `src' and `data'.
# Create and change to a new, empty build directory by running `mkdir build', `cd build'.
# Run `cmake -DDEBUG=ON ..' to create the Makefiles needed to build SuperTux with debug options. If you are missing any libraries needed to build SuperTux, install those first, then try running CMake again. 
# Type `make' to start the build process.
# SuperTux does not need to be installed on the system, you can run it from its own directory.


= Setting up IDEs =

This section is under construction. IDEs that should be able to handle supertux include:

==Kdevelop 4==
You can feed Kdevelop with the CMakeLists.txt. (Project -> Open/Import Project)

==Eclipse with CDT==
* create a build directory '''outside''' of the supertux checkout dir.

Example: Your supertux source is located in <code>~/supertux</code>. You would normally create your build directory <code>~/supertux/build</code> but eclipse seems to fail in that case. So you create <code>~/supertux-build</code>.

* run cmake inside that build directory using the eclipse generator:
    cmake -G"Eclipse CDT4 - Unix Makefiles" /path/to/source

* now open eclipse and select File -> import -> general -> existing project into workspace
* Select your build directory as root directory and click finish.

= Compiling the editor =

== Setup ==

To compile the editor you should make sure that you have some additional dependencies available:

* An already compiled and working svn version of supertux
* mono 1.2.2.1 or newer
* gtk-sharp 2.8

=== Debian ===

Debian users can run the following command to do this:
 apt-get install libgtk2.0-cil libglade2.0-cil libmono-system-runtime2.0-cil mono-gmcs make debhelper pkg-config

If you get an error like
 make: gmcs: command not found
when the editor is compiling, do this as root:
 ln -s /usr/bin/gmcs2 /usr/bin/gmcs

=== Gentoo ===

Gentoo users can use this command:
 emerge -avn ">=dev-lang/mono-1.2.2.1" ">=dev-dotnet/gtk-sharp-2.8.0" ">=dev-dotnet/glade-sharp-2.8.0"
Unmask any packages that might be needed on your arch (none needed on either x86 or amd64).

=== FC6 ===
Just install mono and gtk-sharp2 using yum, and don't forget to install gtk-sharp2-devel (<code>gtk-sharp2-2.10.0-3.fc6</code> and <code>mono-core-1.1.17.1-4.fc6</code> worked fine):
 yum install mono gtk-sharp2 gtk-sharp2-devel
Download the source for the editor into <code>/some/directory/supertux-sharp</code>. For pkgconfig, you need to include <code>/usr</code> in the path, so for bash:
 export PKG_CONFIG_PATH="$PKG_CONFIG_PATH:/usr/"

=== Generic ===

If you have to use the generic installer from the web, be warned that neither the stable(1.1.13) or current(1.1.15_2) have the correct version for gtk-sharp. The recommended way to resolve this is:

1. Install mono using an all-in-one generic installer

The all-in-one installer will try to adjust your environment through the .bashrc file. This is not a proper system-wide change, so (in Slackware at least) modify these scripts and place them in /etc/profile.d

mono.csh

 #!/bin/csh
 setenv PKG_CONFIG_PATH {$PKG_CONFIG_PATH}:/path/to/mono/lib/pkgconfig
 setenv MANPATH ${MANPATH}:/path/to/mono/share/man
 setenv PATH ${PATH}:/path/to/mono/bin

mono.sh

 #!/bin/sh
 export PKG_CONFIG_PATH="$PKG_CONFIG_PATH:/path/to/mono/lib/pkgconfig"
 export MANPATH="$MANPATH:/path/to/mono/share/man"
 export PATH="$PATH:/path/to/mono/bin"

Also, add /path/to/mono/lib in /etc/ld.so.conf
You may have to login again after these changes so they can take affect.

2. Download the source of gtk-sharp at go-mono.com/sources-latest/

3. Compile and install gtk-sharp using "./configure --prefix=/path/to/mono"

4. Verify that the new version is correct by running "pkg-config --modversion gtk-sharp-2.0" (May need to login again for this)

== Building ==

You can compile the editor from commandline with jam. Simply type
 
 make

and the editor will be built. You can then start the editor with

 mono supertux-editor.exe

There are also complete monodevelop project files for the editor in the svn. (TODO write about the hacks needed to actually compile the source in monodevelop).

You might want to read the [[Editor FAQ]] at this point.

=== FC6 ===

In my installation, the editor starts with the following output to the console:
 INFO:  Using configfile: /home/myself/.config/supertux-editor/settings.xml
 INFO:  Supertux is run as: /usr/local/bin/supertux/supertux
 INFO:  Data files are in: /usr/local/bin/supertux/data/
On the first run, these paths were not correctly set, so the editor stopped with an error. The editor offers to set the paths interactively, but that didn't work for me. Instead edit the config file <code>settings.xml</code> itself:
  <LastDirectoryName>/usr/local/bin/supertux/data/</LastDirectoryName>
  <SupertuxExe>/usr/local/bin/supertux/supertux</SupertuxExe>
  <SupertuxData>/usr/local/bin/supertux/data/</SupertuxData>
Yours will probably look differently, and you have to fill in your appropriate paths. Note that <code>LastDirectoryName</code> must exist, otherwise you will run into errors again. Just use the path to data, that should be ok. Do not add any white space between the paths and the tags!

[[Category:Developer documentation]]