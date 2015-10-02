# Small Basic V0.9 is here!

*Vijaye Raji &ndash; 11 June 2010 00:15*

Marking the 300k download milestone, comes the 9th installment of Small
Basic, the fastest and best yet! This version of Small Basic packs a ton
of bug fixes, performance improvements and some of the most requested
features.

Firstly, the Small Basic compiler and runtime have been overhauled and
the result is a big performance gain. Some tight loop programs run up to
4 times faster than the previous versions. This has been the primary
focus of the release.

Next, we have new additions to the library.

- We now have a `Controls` object that allows you to add *Buttons* and
  *TextBoxes* and react to click and text change events.
- The `Shapes` object adds support for adding/modifying, animating, and
  zooming text. This is extremely useful for displaying and updating text
  frequently, like the score in a game.
- The `Sound` object now has a new operation, `PlayMusic`, which plays
  music described by a subset of Music Markup Language supported by
  QBasic. An example is `Sound.PlayMusic(O5 C8 C8 G8 G8 A8 A8 G4 F8 F8 
  E8 E8 D8 D8 C4")`.
  
And then, there are the bug fixes. I won't go into the details but there
are a ton of fixes. An important update is the change in the default
extension for Small Basic documents. Small Basic documents get a default
extension of `.smallbasic` instead of `.sb` to avoid conflicts with MIT's
Scratch.

Last, but certainly not the least, is the support for right-to-left languages
and the first localized language in that series is Arabic. Also included are
Dutch and Polish versions, bringing the count of supported languages to 15!