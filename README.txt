iPhoto plugin for XBMC
======================
This plugin imports an iPhoto library into XBMC.  After importing, you will
see categories that correspond with their iPhoto counterparts:

* Events
* Albums
* Faces
* Keywords
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

* Empty -- albums with no pictures.
* Published -- these are albums pushed to your MobileMe Gallery.
* Flagged -- albums flagged in iPhoto's interface.

Both of these album types are ignored by default.

If you select "Auto update library", the plugin will compare the modification
time of your AlbumData.xml with its current database and update the database
automatically on start.  This is disabled by default.

You can also choose the view style for albums if you're using the Confluence
skin.  You may set this to "Image Wrap," "Pic Thumbs," or "Default".  If you
choose "Default," it will preserve whatever view mode you have chosen in XBMC
for each album; otherwise, it will force the view style to the one selected
here.

Translations
============
If you'd like to help translate this plugin to another language, please send
a patch to jingai at floatingpenguins dot com.

If possible, patch against the most recent version at:

  http://github.com/jingai/plugin.image.iphoto

Known Issues
============
* Sorting by date is broken and therefore disabled for now.
  See http://trac.xbmc.org/ticket/10519
* Need icons for Faces and Keywords.
