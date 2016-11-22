---
title: amenu ![](img/amenu.svg)
...

![Theme default-orange](img/theme/default.png)

About
-----

amenu is a simple and customizable application launcher very much inspired by the excellent [dmenu](http://tools.suckless.org/dmenu/).

Download
--------

There's no installer, simply download and run [amenu.exe](https://github.com/owlnical/amenu/releases/download/v0.3/amenu.exe).

Usage
-----

 1. Press `win + space` to open the amenu interface.
 2. Start typing to search for executables.
 3. Use `←` `→` or `tab` `shift + tab` to change selection.
 4. Press `enter` to launch the selected program.

Settings
--------

There are three separate files for settings available via the tray menu:

 - `paths.ini` - directories to be scanned for .exe files.
 - `hotkeys.ini` - key combinations to show and interact with the GUI.
 - `misc.ini`  - miscellaneous settings.

Theme
-----

There are two variations of the default theme included with amenu.

![Theme default-orange](img/theme/default-orange.png)

![Theme default-red](img/theme/default-red.png)

You can switch theme using the tray menu or by editing misc.ini.

### Create child theme

In the following example we will change the color of the default theme to green by creating a new child theme.

 1. Start by opening the theme directory (tray menu > theme > directory...)
 2. Make a copy of the folder default-orange, name it default-green
 3. Using notepad open the file default-green/gui.css
 4. Change the two color fields from `#fb8c00` (orange) to `#18e072` (green). Your file should now look something like this:

```css
body,div {
	color: #18e072;
}

.selected {
	background-color: #18e072;
}
```

 5. Make sure both lines still end with a semi-colon (`;`)
 5. Save the file and restart amenu (tray menu > restart)
 6. Choose your new theme in the theme sub menu

amenu should now look something like this:

![Theme default-red](img/theme/default-green.png)
 
If you want another color than green you can use this [color picker](https://ddg.gg/?q=color+picker). Simply choose the color you want and copy the value from the bottom text box into gui.css.