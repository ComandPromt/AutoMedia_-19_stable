============================================
Info:
============================================
Plugin Name: AutoMedia for MyBB 1.8.*
->Embeds automatically videos and music from different sites in posts.
->The plugin recognizes the posted URL's and embeds the media. You don't need to insert any MyCode.
->Embed.ly (supports over 400 providers) and Urlembed.com (supports over 5000 providers) are used for embedding.
->Can be enabled/disabled in ACP
->Can be disabled for guests only
->Can be disabled for certain usergroups
->Can be enabled for certain forums only
->Embedding can be disabled by using MyCode tags [amoff]URL[/amoff]
->Embedding can be disabled for signatures (default)
->Embedding can be disabled for quoting posts
->Codebuttons for MyCode can be displayed in editor below textbox.
->Every user can enable/disable embedding in User CP
->Embeds videos and music from many different sites
->Documentation available from plugin overview in ACP
->Embedding of adult video sites can be enabled/disabled
->Embedding of adult video sites can be enabled/disabled for guests only
->Permissions for adult videos can be set by usergroups and forums
->Adult modules are only visible in ACP if adult embedding is enabled
Author: doylecc (http://community.mybb.com/user-14694.html)
Homepage: http://mybbplugins.tk
Version: 4.0.1 (02-11-2018)


============================================
Changelog :
============================================
v4.0.1
#Added: Embedding of several media sites, if no embed service is selected
#Automatic embedding on quick replay improved

v4.0
#Extensive rewrite of the plugin
#Embera and jQuery.Oembed libraries removed
#API for paid embed.ly service removed
#Flash audio player removed
#Urlembed.com service added
#Setting addded for: enable/disable embedding of local links
#Module management in ACP removed. Reason: see next
#Complete embedding function switched from PHP to client-side JavaScript to avoid server load
#Several templates removed
#Several templates modified
#Stylesheet updated
#Table "automedia" removed from database
#Language files updated

v3.1.11
#Bugfix for: Display of active embed libraries in ACP
#Language files updated

v3.1.10
#Bugfix for: Embedded attachments not displayed in portal
#Bugfix for: Embedded media size partially not responsive
#Bugfix for: Embedding of local links
#Template "automedia_head" changed. (Please check "Find updates templates" in ACP)

v3.1.9
#embed.ly Code updated
#Compatibility added for MyBB 1.8.13 URL's using rel="noopener"

v3.1.8
#Restore automedia.css for Master Style on activation

v3.1.7
#HTTPS support for several modules added
#Several embed codes updated

v3.1.6
#Bugfix for: If "embed.ly free" is enabled, the settings for signatures and quotes are not respected
#Bugfix for: Due to a missing line in template automedia_head, the max-width setting isn't applied

v3.1.5
#Bugfix for: Error message on opening a new thread, if forum rules are displayed in thread list
#New settings option added for using embed.ly for free without API key
#New settings option added for Embera and oEmbed libraries
#Admin language file updated
#Template updated
#CSS elements moved from template to own theme stylesheet (automedia.css)
#Uninstall option added for deleting plugin files
#Mediaelement player updated to version 3.2.4
#Bugfix for: [amoff] tags with attachments visible in posts

v3.1.4
#Bugfix for: permission handling in attachment module
#Bugfix for: max-width and max-height settings not applied
#Mediaelement player updated to version 3.2.3

v3.1.3
#Embedding of video and audio attachments in posts added
(Attachments have to be inserted into the post for embedding e.g. [attachment=123])
#Setting für displaying download links of embedded attachments added

v3.1.2
#Fullscreen mode for Mediaelement player added
#Bugfix for: quick jump arrow in quotes isn't displayed

v3.1.1
#Mediaelement player updated to version 3.0.0
#Language files updated
#Fixed: mp3 module causing server error with PHP version 5.4.* and older

v3.1.0
#Mediaelement player updated to version 2.23.4
#Embera updated to version 1.9.3
#Audio Playlist function replaced
#Several templates updated
#Several embed codes updated
#Fixed: compatibility with MyBB 1.8.8 parser

v3.0.3
#CDN support added
#several templates updated
#PHP version check added
#Mediaelement player updated to version 2.16.3
#Embera updated to version 1.8.5
#Embed.ly jQuery script updated to version 3.1.2

v3.0.2
#Video count in postbit fixed

v3.0.1
#Code optimizations
#2 templates updated
#Mediaelement player updated to version 2.16.1
#Embera updated to version 1.8.4
#Improved HTTPS support
#Embedly in print thread and archive fixed

v3.0
#HTML elements moved from plugin files to templates
#Consistent use of language strings
#Several Settings in ACP added and replaced
#Use of oEmbed API for embedding - embed codes stay up to date
#Embed.ly service can be used with valid API Key
#HTML5 Mediaelement player with Flowplayer as flash fallback

v2.3
#Plugin compatible with MyBB 1.8 (only)



============================================
Installation :
============================================
1. Upload the complete content of the Upload folder into your forum home directory
   (For additional languages you have to upload the language files too.)
2. Go to your "AdminCP Configuration - Plugins" and click "Install & Activate" behind AutoMedia
3. After activation you'll find a new settinggroup "AutoMedia Global" in "ACP - Configuration - Settings".
   Here you can generally enable/disable embedding without losing your settings.
   You can also disable embedding only for guests or for other usergroup(s) as well.
   Embedding can be enabled for certain forums only here too.
   Embedding of adult videos can be enabled (disabled by default)
   Permissions for adult videos can be set by usergroups and forums
   Embedding can be disabled in signatures (default)
   Max. width and height of embedded files
   Embed.ly oEmbed service can be activated and API Key can be inserted.
   Codebuttons can be enabled/disabled for MyCode
   Embedding can be disabled for quoting posts
4. The plugin adds in "User CP" a new menu item "AutoMedia."  In "AutoMedia" you'll find radio buttons. Every user can set whether he wants embedding enabled (Yes (default)) or disabled (No). If he chooses "No" he will only see the links in posts instead the embedded media.
5. All done.


============================================
Update from versions 3.*:
============================================
1. Upload the complete content of the Upload folder into your forum home directory and overwrite the existing files.
2. In ACP -> Configuration -> Plugins deactivate AutoMedia and activate it again.
3. In ACP -> Templates & Style -> Templates -> run Find Updated Templates. If there are any automedia templates listed, revert them (and possibly reinsert your own code.)
4. All done


============================================
Update from all older versions:
============================================
1. Deinstall the old AutoMedia plugin
2. Upload the complete content of the Upload folder into your forum home directory and overwrite the existing files.
   For additional languages you have to upload new language files too.
3. see "Installation" beginning with #2



============================================
List of Media:
============================================
-The Embed.ly service currently supports over 400 providers

-The Urlembed.com service currently supports over 5000 providers

-Additionally 14 different adult video sites (disabled by default) are supported

-Supported file types:
# MP3/M4A/WAV/OGG audio and MP3 Playlist
# MP4/M4V/MP4V/OGV/WEBM video
# FLV Flash video
# SWF Flash
# DivX video
# AVI video
# MKV video
# MOV Quicktime video
# RM/RAM/SMIL/RV/RPM Real media
# WMV/WMA Windows media
# MPG/MPEG video

Please note that you need to have all necessary plugins/addons installed in your webbrowser to embed all media file types!

============================================
cURL support:
============================================

With AutoMedia 4.0 cURL and fsockopen aren't required anymore. All embedding is handled client side.


============================================
Disclaimer:
============================================
This program is free software: you can redistribute it and/or modify
    it under the terms of the GNU General Public License as published by
    the Free Software Foundation, either version 3 of the License, or
    (at your option) any later version.

    This program is distributed in the hope that it will be useful,
    but WITHOUT ANY WARRANTY; without even the implied warranty of
    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
    GNU General Public License for more details.

    You should have received a copy of the GNU General Public License
    along with this program.  If not, see <http://www.gnu.org/licenses/>
