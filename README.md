# xna

_Most of these classes should be stand-alone and you should be able to copy and paste them straight in to your XNA projects. If any of the classes rely on one or more other of my classes then I'll specify in the file description._

#### Sprite.cs

A wrapper class that helps with drawing textures with various transformations simplified for example you can specify a sprite width and height, or specify a scale to apply to the texture's default dimensions. This basically just takes all of the arguments for spriteBatch.Draw() and wraps it up into a class.

#### Screen.cs

A manager-style class that helps with changing the screen size while keeping the game logic the same. It automatically fits the game's viewport to the screen (while preserving aspect ratio) and keeps a record of the game's 'virtual' dimensions for the game's logic. Also calculates the view matrix every time the game dimensions are changed which should be used with spriteBatch.Begin().
