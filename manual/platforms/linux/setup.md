# Requirements

To develop for Linux using Xenko, you need a Linux PC with a graphic card that supports at least OpenGL 4.2 or Vulkan 1.0. The preferred Linux distribution for Xenko is Ubuntu 16.04 or later, as this was the setup we used to develop the Linux version of Xenko.

The instructions below assume you have Ubuntu 16.04 installed. You might need to adapt them according to your Linux distribution.

You will also need a Windows PC to build your projects for Linux using Game Studio.

## Setup

You need the following packages:

* [FreeType](#freetype)

* [OpenAL](#openal)

* [SDL2](#sdl2)

* either Mono or .NET Core (it's OK to install both)

## FreeType

To render fonts, we use the [FreeType](https://www.freetype.org/) library. The minimum required version is 2.6 and can be installed via:

```
sudo apt-get install libfreetype6-dev
```

## OpenAL

To play sounds and music, we use the [OpenAL](https://www.openal.org/) library. It can be installed via:

```
sudo apt-get install libopenal-dev
```

## SDL2

To run games on Linux, we use the [SDL2](https://www.libsdl.org/) library which provides the ability to create windows, handle mouse, keyboard and joystick events. The minimum required version is 2.0.4 and can be installed via:

```
sudo apt-get install libsdl2-dev
```

## Mono

To install Mono, please refer to the [Mono Project](http://www.mono-project.com/docs/getting-started/install/linux/) installation instructions for Debian/Ubuntu. 

Make sure version 4.4 is installed. To check which version you have installed, type:

```
mono --version
```

### .NET Code

For information about how to install .NET Core, see the [.NET Core instructions for Debian/Ubuntu](https://www.microsoft.com/net/core#ubuntu). 

Make sure version 1.0 is installed. To check which version you have installed, type:

```
dotnet --version
```
