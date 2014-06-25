# SDL2 boilerplate project

This is a simple project containing a basic CMake build system configuration in
order to compile SDL2 projects written in C.

Supports SDL2 but also its popular extensions such as SDL_image, SDL_mixer and
SDL_ttf so you can directly use them in your project.

## Building

Simply run the following commands in order to build the example program :

    :::console
    $ mkdir build
    $ cd build/
    $ cmake ..
    $ make

Then, you can run it (it will display a window with 3 color lines) :

    :::console
    $ ./test

## Adapting configuration

You may need to modify the `CMakeLists.txt` file in order to adapt the build
system for bigger projects. For further informations, please read the CMake
documentation.

## Copyright

This project is brought to you under WTFPL. For further informations, please
read the COPYING file.
