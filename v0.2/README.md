# Announcing Small Basic v0_2!

*Vijaye Raji &ndash; 17 December 2008 09:00*

As promised, we have a new release of Small Basic! This version contains
all the most requested features by the user community. Thanks everyone for
the great suggestions and for making Small Basic better and better! Please
keep the feedback flowing. We're listening.

For those that are new, Microsoft Small Basic is a project that aims at
bringing the fun back to programming and encourages everyone, from kids to
adults to take their first step into the wonderful world of programming.

At a high level, this release includes the following updates:

- Bug fixes on the IDE
- A smarter compiler with better language service features, including
  auto-indent
- Inclusion of `ElseIf` keyword in the language
- Better File access operations
- Access to position and angle of Turtle

Here's a complete list of all the updates

- **Language and Editor**  
   - Several Crash fixes
   - Support for non-US regional OS settings
   - Auto-indent
   - Parentheses for conditional expressions are now optional
   - Added `ElseIf` keyword to the language
   - Support for inline comments
   - Fixed bug with negative step value in `For..EndFor`
- **Library API Additions**
   - **Array**
      - `GetItemCount`
      - `ContainsIndex`
      - `ContainsValue`
      - `RemoveValue`
   - **Desktop**
      - Get `ScreenWidth` and `ScreenHeight`
   - **File**
      - `CreateDirectory`
      - `DeleteFile`
      - `GetFiles`
      - `GetDirectories`
      - `WriteContents` *Fix: Now works even if the file doesn't already
        exist*
   - **GraphicsWindow**
      - Performance improvements
      - `Width`/`Height` *Fix: No need to set these twice*
      - `Hide` *Fixed crash*
      - `Add/FillTriangle`
      - `RotateShape`
      - `CanResize` *You now have the option of changing the resize mode*
      - `Left/Top` *You can now position the window*
      - `GetColorFromRGB` *Construct a valid color value from the color components*
   - **Math**
      - `Power`
      - `GetRandomNumber` *Fix: Is one based and includes the max-number in range.
        **[Breaking Change]***
   - **Program**
      - Fixes for `End()`
      - `ProgramDirectory` *Gets the directory of the program*
   - **Text**
      - `Append` *For those times when you want a number to be treated as text*
      - `GetCharacter` *Unicode character code to Character*
      - `GetCharacterCode` *Character to Unicode Character code*
   - **TextWindow**
      - `Clear`
      - `Left/Top`
   - **Turtle**
      - `Angle`
      - `X`, `Y`