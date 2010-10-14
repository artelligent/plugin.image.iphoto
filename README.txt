iPhoto plugin for XBMC
======================
This plugin imports an iPhoto library into XBMC.  After importing, you will
see three categories that correspond with their iPhoto counterparts:

* Events
* Albums
* Ratings

Configuration
=============
The plugin needs to know where your AlbumData.xml file is.  If you haven't
explicitly pointed iPhoto to a non-standard library location, the default of
"~/Pictures/iPhoto Library/AlbumData.xml" should work fine.  Otherwise,
please enter in the correct path in the plugin's settings dialog.

The iPhoto plugin can also be configured to ignore certain album types.
It is currently hard-coded to ignore albums of type "Book" and
"Selected Event Album," but you can choose to ignore also:

* Published -- these are albums pushed to your MobileMe Gallery.
* Flagged -- albums flagged in iPhoto's interface.

Both of these album types are ignored by default.

If you select "Auto update library", the plugin will compare the modification
time of your AlbumData.xml with its current database and update the database
automatically on start.  This is disabled by default.

Translations
============
If you'd like to help translate this plugin to another language, please send
a patch to jingai at floatingpenguins dot com.

If possible, patch against the most recent version at:

  http://github.com/jingai/plugin.image.iphoto

Known Issues
============
* No support for Keywords and Faces (yet).
