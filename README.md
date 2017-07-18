# xna

A bunch of written in C# for use in XNA 4.0 Windows Game projects.

_Most of these classes should be stand-alone and you should be able to copy and paste them straight in to your XNA projects. If this is not the case I'll specify the dependencies in the file description and below. All classes have been prefixed with 'GM\_' so they don't clash with any existing files but if you want to remove them just rename the class and file before using. Please also note that all the files have been __heavily__ commented. I would massively appreciate it if you would contact me upon finding any shotfalls or errors with my code, or if you simply have a suggestion to improve it and its functionailty!_

***

### Contents
[GM_Sprite.cs](#gm_sprite)<br>
[GM_Screen.cs](#gm_screen)<br>

***

<a name="gm_sprite"/>

#### [GM_Sprite.cs](https://github.com/george-mcdonagh/xna/blob/master/GM_Sprite.cs)

A wrapper class that helps with drawing textures with various transformations simplified for example you can specify a sprite width and height, or specify a scale to apply to the texture's default dimensions. This basically just takes all of the arguments for spriteBatch.Draw() and wraps it up into a class.

<a name="gm_screen"/>

#### [GM_Screen.cs](https://github.com/george-mcdonagh/xna/blob/master/GM_Screen.cs)

A manager-style class that helps with changing the screen size while keeping the game logic the same. It automatically fits the game's viewport to the screen (while preserving aspect ratio) and keeps a record of the game's 'virtual' dimensions for the game's logic. Also calculates the view matrix every time the game dimensions are changed which should be used with spriteBatch.Begin().
