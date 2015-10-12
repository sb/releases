# Small Basic v1.2 Release Notes

*These notes have been taken from the Official Microsoft Download Center
page for Small Basic 1.2, and were not originally included in the blog post
announcing Small Basic 1.2. The copy of the announcement blog post can be
found [here](./README.md).*

### New Features

1. **Kinect for Small Basic** &ndash; Small Basic 1.2 introduces three
   Kinect objects: `KinectBodyList`, `KinectFaceList`, and `KinectWindow`.
   With these objects, you can program with the Microsoft Kinect Sensor
   and the information that it captures. You can:
   
    - Show the color, infrared, depth, body index, and body sensor data.
    - Capture images from the color, infrared, depth, and body index
      sensors.
    - Replace the background behind people in the foreground with another
      image (this is similar to chroma key compositing or "green screen"
      processing).
    - Get the position and orientation of 26 different "joints" in up to
      6 human bodies in both 3D space and on the screen.
    - Get the open/closed state of the hands of up to 6 humans in front
      of the sensor.
    - Get the lean angle of up to 6 humans in front of the sensor.
    - Get the position and orientation of the faces of up to 6 humans in
      front of the sensor.
    
2. **Dictionary Object: Expanded Languages** &ndash; In Small Basic 1.0,
   the `Dictionary` object supported the following languages (where you
   enter a word in the first language and the definition is displayed in
   the second language): `EnglishToEnglish`, `EnglishToFrench`, and
   `FrenchToEnglish`. We expanded our support to these languages:
   
    - `EnglishToGerman`, `GermanToEnglish`
    - `EnglishToItalian`, `ItalianToEnglish`
    - `EnglishToJapanese`, `JapaneseToEnglish`
    - `EnglishToKorean`, `KoreanToEnglish`
    - `EnglishToSimplifiedChinese`, `SimplifiedChineseToEnglish`
    - `EnglishToTraditionalChinese`, `TraditionalChineseToEnglish`
    - `EnglishToSpanish`, `SpanishToEnglish`


### Bug Fixes

- **Dictionary Object (1.0-12)** &ndash; The Dictionary site changed their
  API, which broke the `Dictionary` Object for Small Basic 1.0 and 1.1. This
  has been fixed for Small Basic 1.2.
- **Language Improvements** &ndash; We made thorough reviews and updated the
  UI text for these languages: Chinese (Simplified), Chinese (Traditional),
  Czech, Dutch, French, German, Hebrew, Italian, Japanese, Portuguese (Brazil),
  Portuguese (Portugal), Russian, Spanish, and Turkish. We also had some logged
  errors that were fixed in this pass:  
   - **Hebrew Errors (1.0-D03)** &ndash; Hebrew translation errors in the IDE are
     fixed.
   - **French Errors (1.0-D05, D06, D07)** &ndash; French translation errors in
     the IDE are fixed.
   - **Japanese Errors (1.0-D01, D12-28)** &ndash; Japanese translation errors in
     the IDE are fixed.    
- **`GraphicsWindow.GetPixel` Crash (1.0-14)** &ndash; In Small Basic 1.0/1.1, the
  `GraphicsWindow.GetPixel` method crashed if the coordinates were outside the
  window (such as `x < 0`). This crash is eliminated in 1.2.
- **`Turtle.Show()` Issue (1.0-02)** &ndash; In Small Basic 1.0/1.1, the
  `Turtle.Show()` method didn't show the Turtle after you used `Graphicswindow.Clear()`
  or `Turtle.Hide()`. This has been fixed for 1.2.
- **`Textwindow.Show` Crash (1.0-15)** &ndash; In Small Basic 1.0/1.1, hiding and
  showing a `TextWindow` crashed (Windows 8.1) and deleted content (Windows 7). This
  crash is eliminated in 1.2.
- **Setup Needs .NET Framework 3.5 SP1 (1.1-01)** &ndash; In Small Basic 1.1, the
  Small Basic Setup (`SmallBasic.en_us.msi`) requires you to have .NET Framework
  3.5 SP1 installed. This is inconsistent because Small Basic v1.1 moves to the
  requirement of .NET Framework 4.5 instead. This has been fixed for 1.2.
- **`Shapes.AddText()` Error (1.0-05)** &ndash; In Small Basic 1.0/1.1, if you use
  the `Shapes.AddText()` method at the top of your program, Small Basic shows an
  exception thrown by the target. The exception is no longer thrown in 1.2.
- **`Math` Object Crashes (1.0-03)** &ndash; In Small Basic 1.0/1.1, various `Math`
  object errors caused unhandled exceptions. The crashes were fixed for 1.2.
- **Divide By Zero Produces Zero (1.0-22)** &ndash; In 1.0/1.1, if you divide by
  zero (`0`), you get the result of zero (`0`), even though in math this isn't
  possible (and should result in an error). In 1.2, you receive an error when you
  attempt to divide by zero.
- **IDE Documentation Updates** &ndash; We made several improvements to keep the
  documentation in the UI as accurate as possible:
   - **`Math.Floor` and `Math.Ceiling` (1.0-D04)** &ndash; Clarified how these
     return the largest integer.
   - **`Control.Add*()` Methods (1.0-D08)** &ndash; Updated to mention how they
     require the position coordinates not the width/height.
   - **`Network` Object (1.0-D09)** &ndash; Clarified that it is a helper class,
     not a private helper.
   - **`Sound.PlayMusic` (1.0-D10)** &ndash; Updated "MML" to write out as
     "Music Macro Language".
     
     
### Breaking Changes to `v1.0`

There are no new breaking changes introduced in Small Basic 1.2. However, there
are two breaking changes from Small Basic 1.1 that break Small Basic 1.0:

1. **Windows XP** &ndash; Due to the upgrade to .NET Framework 4.5, Small Basic
   1.1/1.2 does not work on Windows XP and older operating systems. We will
   continue to offer Small Basic 1.0 for users of Windows XP and older operating
   systems.
2. **1.0 Extensions** &ndash; All extensions built for Small Basic 1.0 will need
   to be recompiled on Small Basic 1.1/1.2 and re-released. Extensions built on
   1.1 will work fine on 1.2.
   
   
### Updates made in `v1.1`:

1. **.NET Framework 4.5** &ndash; We upgraded to .NET Framework 4.5 from 3.5.
   Although this causes some breaking changes (see below), it's necessary in
   order to build out new objects that take advantage of new devices, operating
   systems, and capabilities.
2. **Modernized UX: Controls** &ndash; The design of the program controls (button,
   scroll bar, arrows on the control bar) in the `GraphicsWindow` is now 
   flat/modernized. This includes blue and dark gray borders around the text boxes.
   And the window title font is also updated.
3. **Language Downloads** &ndash; You can now directly download your language from
   the Download Center. See the 
   [Download Center Page](https://www.microsoft.com/en-US/download/details.aspx?id=46392).
   
   
### Bug Fixes made in `v1.1`:

1. **`Flickr` Object (1.0-17)** &ndash; Flickr changed their API, which broke the 
   `Flickr` Object. This has been fixed for Small Basic 1.1.
2. **Find + Arrow Keys Crash (1.0-21)** &ndash; In 1.0, the Small Basic environment 
   hangs up (shows "Not Responding") when pushing arrow keys while text finding when 
   you have multiple edit windows open. This issue is fixed in 1.1 and can no longer 
   be reproduced.