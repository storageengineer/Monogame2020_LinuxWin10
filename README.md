# Monogame Template
Monogame 3.8 + Visual Studio Community Edition 2019 (VSCE2019) + Game State Management

During the summer of 2020, I took up game programmming.  For some reason I thought it would be easy to pick up on game delevopment and learn C# (and VSCE2019) at the same time.

I chose Monogame as the game engine, mostly for cross platform Linux support.  Plus I have and old book on how to write games with XNA--Monogame is a current game engine that is XNA compatible.

Wrote my first "game" which consisted of moving around an object and bouncing off the walls.  As soon as I added points, I had a problem.  How do I display the top 10 high scores?  The only game state was playing the game; as soon as you start the program, you're playing the game.  When your health gets to zero, you stop moving.  There was no other game state for game intro, player death, or a game over state.

My one book solved the problem with an enum of possible game states and a huge switch statement.  I'm looking as the switch statement and thinking, "Theres got to be a better way" right along with "They published a giant case statement as a solution?!"  XNA is _not_ a new game engine, other people have run into these issues, how did _they_ solve it?

An object oriented stacked game state manager.  Microsoft released the code and sample demo of the game state manager, the original site is gone but it was successfully [replicated to Github.](https://github.com/tomizechsterson/game-state-management-monogame)

Step 1, write  _something!_  And I did, a nice little space shooter not unlike the classic asteroids game.  Barely playable, terrible graphics (circles and a triangle),and no sound but it was a start.
Step 2, improve what you wrote in step 1.  Well, my little shooter drops you in the middle of the game as soon as the program starts.  A simple intro, pre-game menu, and post game hi scores with credits would be an excellent addition.
Step 3, Google a solution since this is _not_ a new problem.


Right there, on step 3, I kept hitting roadblocks.  More than a few articles online started with creating an enum for the game states and then using a giant switch statement in the update/draw methods.  If you only have three game states, that's maintainable but anything more complex and you're going to end up with a FSM inside your update/draw methods.  Now you can tweak this approach all kinds of ways to improve performance or maintainability, but you're still tweaking a bad solution.





While learning some basics of Monogame, I ran into the issue of game state management early on.  A lot of resources online show an enum of game states and a nightmarish switch statement inside their draw and update methods.  This is not a maintainable, sustainable, or suitable way to handle game states

A bit more Googling and I ran into a [Windows Game State Manager](https://marketplace.visualstudio.com/items?itemName=XNAGSEducation.WindowsGameStateManagement&ssr=false#overview) template for Visual Studio.  Bad news is that its for an older version of Visual Studio and I wasn't able to import the template into VSCE2019, something in the vsix file wasnt compatible.  Good news, I'm persistent.

Renamed, unzipped, and extracted the template code files.  Created a solution in VSCE2019 with Monogame 3.8 and the code files dug out of the template.
