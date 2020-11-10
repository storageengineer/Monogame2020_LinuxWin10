# Monogame Template
Monogame 3.8 + Visual Studio Code + Stacked Game State Management + Compile to Linux, Win10, and Mac(1)!


While learning the basics of Monogame, I ran into the issue of game state management.  A bit more Googling and I ran into a [Windows Game State Manager](https://marketplace.visualstudio.com/items?itemName=XNAGSEducation.WindowsGameStateManagement&ssr=false#overview) template for Visual Studio.  GSM solution written by Microsoft, packaged as a VS template by XNA GS.  The template was designed for an older version of Visual Studio (2010 I think) and links to the XNA assembly, making it incompatible with Monogame and Visual Studio Code.

Renamed, unzipped, and extracted the template code files.  The C# files contain the code I need, I can add them to a new Monogame project without copying the XNA assembly dependencies.  The results you now see in this repository.

-----

This is a Monogame v3.8, Desktop GL project.  C# files were added to the project manually and the /contents folder was rebuilt manually.  Cross compiling following the Monogame docs let me build a Win64 version that works.  Code was written for and tested on Ubuntu 20.04 LTS, and the Win64 build ran successfully on a Windows 10 VM.

*Make sure you edit the gamefonts.spritefont and menufonts.spritefont to use a font on your system.  Currently its set to Arial font.*

There's no dependencies to the original XNA assemblies nor does it reqire an old version of Visual Studio.  Code will download Monogame components via nuget as needed.

(1) While I can test the ability to build and run successfully on Android (planned), Linux, and Windows 10, I am unable to test any Mac or iOS builds.  I do not own any Apple devices.  As always, these guidelines are just that, guidelines.  
