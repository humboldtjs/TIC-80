![TIC-MSX](https://tic.computer/img/logo64.png)
**TIC-MSX TINY COMPUTER** - [https://tic.computer/](https://tic.computer/)

# About
TIC-MSX is a **FREE** and **OPEN SOURCE** fantasy computer for prototyping games for an MSX (and making, playing and sharing tiny games), with roughly the specs of an MSX1 computer.
With TIC-MSX you get built-in tools for development: code, sprites, maps, sound editors and the command line, which is enough to create a mini retro game.

Games are packaged into a cartridge file, which can be easily distributed. TIC-80 works on all popular platforms. This means your cartridge can be played in any device.

To make a retro styled game, the whole process of creation and execution takes place under some technical limitations: 240x136 pixel display, 16 color palette, 256 8x8 color sprites, 4 channel sound, etc.

![TIC-MSX](https://user-images.githubusercontent.com/1101448/29687467-3ddc432e-8925-11e7-8156-5cec3700cc04.gif)

### Features
- Multiple programming languages: [Lua](https://www.lua.org),
  [Moonscript](https://moonscript.org),
  [Javascript](https://developer.mozilla.org/en-US/docs/Web/JavaScript),
  [Wren](http://wren.io/), and [Fennel](https://fennel-lang.org).
- Games can have mouse and keyboard as input
- Games can have up to 4 controllers as input (with up to 8 buttons, each)
- Built-in editors: for code, sprites, world maps, sound effects and music
- An aditional memory bank: load different assets from your cartridge while your game is executing

# Binary Downloads
You can download compiled versions for the major operating systems directly from our [releases page](https://github.com/humboldtjs/TIC-MSX/releases).

# Pro Version
TIC-MSX is based on TIC-80. If you want to support TIC-80 (and by extension TIC-MSX) development, the guys from nesbox have a [PRO Version](https://nesbox.itch.io/tic).
This version has a few additional features and binaries can only be downloaded on [their Itch.io page](https://nesbox.itch.io/tic).

See [TIC-80](https://github.com/nesbox/TIC-80) for more information.

# Contributing
You are can contribute by issuing a bug or requesting a new feature on our [issues page](https://github.com/nesbox/TIC-MSX/issues).
You can also contribute by reviewing or improving our [wiki](https://github.com/nesbox/TIC-MSX/wiki).

See [TIC-80](https://github.com/nesbox/TIC-80) for more information.

# Build instructions

## Windows
### with Visual Studio 2017
- install `Visual Studio 2017`
- install `git`
- run following commands in `cmd`
```
git clone --recursive https://github.com/humboldtjs/TIC-MSX
cmake -G "Visual Studio 15 2017 Win64"
```
- open `TIC-80.sln` and build
- enjoy :)

### with MinGW
- install `mingw-w64` (http://mingw-w64.org) and add `.../mingw/bin` path to the *System Variables Path*
- install `git`
- install `cmake` (https://cmake.org)
- run following commands in `terminal`
```
git clone --recursive https://github.com/humboldtjs/TIC-MSX
cd TIC-MSX
cmake -G "MinGW Makefiles"
mingw32-make -j4
```

## Linux 
### Ubuntu 14.04
run the following commands in the Terminal
```
sudo apt-get install git cmake libgtk-3-dev libgles1-mesa-dev libglu-dev -y
git clone --recursive https://github.com/humboldtjs/TIC-MSX && cd TIC-MSX
cd build
cmake ..
make -j4
```

to install the latest CMake:
```
wget "https://cmake.org/files/v3.12/cmake-3.12.0-Linux-x86_64.sh"
sudo sh cmake-3.12.0-Linux-x86_64.sh --skip-license --prefix=/usr
```

### Ubuntu 18.04

run the following commands in the Terminal
```
sudo apt-get install git cmake libgtk-3-dev libglvnd-dev libglu1-mesa-dev freeglut3-dev -y
git clone --recursive https://github.com/humboldtjs/TIC-MSX && cd TIC-MSX
cd build
cmake ..
make -j4
```

## Mac
install `Command Line Tools for Xcode` and `brew` package manager

run the following commands in the Terminal
```
brew install git cmake
git clone --recursive https://github.com/humboldtjs/TIC-MSX && cd TIC-MSX
cd build
cmake ..
make -j4
```

## iOS / tvOS
You can find iOS/tvOS version here 
- 0.60.3: https://github.com/brunophilipe/TIC-80
- 0.45.0: https://github.com/CliffsDover/TIC-80
