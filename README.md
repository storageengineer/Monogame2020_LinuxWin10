# Monogame Template
Monogame 3.8 + Visual Studio Community Edition 2019 (VSCE2019) + Stacked Game State Management

While learning the basics of Monogame, I ran into the issue of game state management.  A bit more Googling and I ran into a [Windows Game State Manager](https://marketplace.visualstudio.com/items?itemName=XNAGSEducation.WindowsGameStateManagement&ssr=false#overview) template for Visual Studio.  GSM solution written by Microsoft, packaged as a VS template by XNA GS.  The template was designed for an older version of Visual Studio and links to the XNA assembly, making it incompatible with Monogame and VSCE2019.

Renamed, unzipped, and extracted the template code files.  The C# files contain the code I need, I can add them to a new Monogame project without copying the XNA assembly dependencies.  The results you now see in this repository.

-----

This is a Monogame v3.8, Desktop GL project.  C# files were added to the project manually and the /contents folder was rebuilt manually.

Make sure you edit the gamefonts.spritefont and menufonts.spritefont to use a font on your system.  Currently its set to Arial font.

There's no dependencies to the original XNA assemblies nor does it reqire an old version of Visual Studio.

If I learn how to create a VS2019 Template addon, I'll add that to this repository
