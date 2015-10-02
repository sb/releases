# Microsoft Small Basic v0.3 is here

*Vijaye Raji &ndash; 10 Feb 2009 13:55*

The next iteration in Microsoft Small Basic's pre-release cycle is here.
Once again, we've taken feedback from the community and are giving you
what you asked for. So, don't forget to request your favourite feature
in our [forums](http://social.msdn.microsoft.com/Forums/en-US/smallbasic/threads/).

This release features a few features, a bunch of bug fixes and a couple
important breaking changes. Please note these breaking changes because
you would have to update some of your programs before they would work in
the new version.


### First, the features

1. **Publish and Import**  
   Remember how you had to copy and paste your program to share it with friends
   or to post your sample on the forums? Well, you don't have to anymore. Just
   hit the **Publish** button and you'll get back a 6-digit/letter combination
   code. This code uniquely identifies your program and your friends can now
   view and run your program by importing it using this code.  
     
   Also, you can view your program by going to 
   [smallbasic.com/program/](http://smallbasic.com/program/) and typing your
   program code. For example, I wrote a really simple program and published it.
   The id I got back was `DCT967`. Everyone can now view this program at:
   [smallbasic.com/program/?DCT967](http://smallbasic.com/program/?DCT967)
2. **Splash Screen**
3. **Performance optimizations**: Makes Small Basic startup faster.


### Bug Fixes

1. Fixed a lot of regional formatting issues. Decimals now preserve their
   precision in non-US settings machine.
2. Fixed issues with `DateTime` formatting in non-US settings machine.
3. Fixed Font Size issues. Font Sizes can now be set once and they take
   effect right away.
4. Fixed issues with multiple event subscribers. There can now only be one
   sub routine subscribed to an event now.
5. Added Close Button to the errors window
6. Added sync lock for `CreateWindow` in `GraphicsWindow` object. Extenders
   can now run multi-threaded if they want to.
7. Program now exits cleanly after setting the desktop background.
8. `GetHeight` and `GetWidth` on `ImageList` now return the correct pixel
   height and width respectively.
9. Fixed crash that happens when permission to the temporary folder is denied.


### Breaking Changes

Here is a list of breaking changes in `v0.3`. These are important because you
might have to update some of your programs to run on this.

1. **Shapes object:** The `GraphicsWindow` has been factored out and there's
   now a `Shapes` object. This object contains operations like `AddRectangle`,
   `AddEllipse`, etc. These methods used to be on `GraphicsWindow` and now
   they are no more. If your program used them, you'd have to modify your
   program to match the new pattern.
2. **ImageList.LoadImage:** `ImageList.LoadImage` no longer takes an "image id"
   as an argument. Instead it returns a newly created id for you to use. For
   example, `pic = ImageList.LoadImage("c:\myimage.jpg")`.