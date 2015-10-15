This repo is based on work done from learnopengl.com  modified to fit an Xcode environment
(why do all the tutorials insist on using Visual Studios?  I mean... its ok.... if you like clicking GUIs.)

-on that note, here's some instructions on what GUI components to click.

Couple notes to get this working locally, if you're ummm... NOT ME

1. You'll need to install the "glew" library and the "glfw3" library, to do this, use brew.

2. If you don't know about brew, google it.

3. after install, go to your project, click on "Build Phases" > "Link Binary with Libraries".

4. click the plus sign, then click "Other" button.  Press Shift + Commmand + G (this hotkey combo allows you to pick your path for the library).

5. Locate the libGLEW and libglfw3 .dylib files and click them, usually located in /usr/local/Cellar.... blah blah blah (since you used brew, if you didn't punch yourself).

6. Go to Build Settings > Search Paths

7. Add "/usr/local/include" and "/opt/local/include" to the Header Search Paths category.

8. The Library search paths (the path to your lib files) should already be set, but double check that they're correct just to make sure.

9. This is a pretty standard way of adding libraries to a Xcode project, if there's a library that I didn't leave instructions for (ie. SOIL) use the same steps, notably 3-8.  Because you know honestly, sometimes brew doesn't have the libraries you need. 