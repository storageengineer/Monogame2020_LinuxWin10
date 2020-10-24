# Monogame Template
Monogame 3.8 + Visual Studio Community Edition 2019 (VSCE2019) + Game State Management

During the summer of 2020, I took up game programmming.  For some reason I thought it would be easy to pick up on game delevopment and learn C# (and VSCE2019) at the same time.

While learning the basics of Monogame, I ran into the issue of game state management early on.  A lot of resources online show an enum of game states and a nightmarish switch statement inside their draw and update methods.  Thats a bad idea, more than 3 states and you're putting a FSM in you draw/update loops.

A bit more Googling and I ran into a [Windows Game State Manager](https://marketplace.visualstudio.com/items?itemName=XNAGSEducation.WindowsGameStateManagement&ssr=false#overview) template for Visual Studio.  Bad news is that its for an older version of Visual Studio and I wasn't able to import the template into VSCE2019, something in the vsix file wasn't compatible.

Renamed, unzipped, and extracted the template code files.  Created a solution in VSCE2019 with Monogame 3.8 and the code files dug out of the template.

This repository is what I ended up with.

This is a Monogame v3.8, Desktop GL project.  C# files were added to the project manually and the /contents folder was rebuilt manually.  There's no references to the original XNA assemblies or old Visual Studio solution/project files.
