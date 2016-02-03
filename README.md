# Music-video-nfo-generator

This is a visual basic script for use in MediaMonkey 4
The purpose of this script is to create *.nfo files for use in Kodi (should work in all versions)

Usage:
Download from the releases tab MV_nfo_generator.mmip (this is just a zip file for MediaMonkey)
1.  Start MediaMonkey and use menu Tools - Extensions... to open the Extensions dialog
2.  Click the "Add..." button and browse to your download location ffor the mmip file and select it.
3.  MediaMonkey should install the script automatically

Alternatively, you can open MV_nfo_generator.mmip in an unzip program and manually extract the files to your
Windows user %APPDATA% MediaMonkey folder and place the files in the Scripts subfolder.  Then open 
 MV_nfo_generator.vbs in a text editor and copy the required script.ini lines and paste them into your local 
 copy of scripts.ini
 
 First run:
 The script is run by using the MediaMonkey menu File -- Create reports and select MV nfo generator ... from the 
 drop-down select list.   You should have one or more music video files visible and selected in the main MediaMonkey 
 window.  The nfo files will be created for the selected files.  On ffirst run of the script, you will need to load one of
 the two configuration files provided with the script.  These files are designed to extract data from the MediaMonkeylibrary 
 and convert them for Kodi.  If you installed the script using the auto method, these files will be located in your local
 %APPDATA% MediaMonkey Scripts folder.  Alternatively they can be extracted from the mmip zip file and placed where
 desired.
 
 Using the "load" button in the script dialog, select one of the two files.  They differ as follows:
 musicvideo_albumartist_nfo.dat uses the artist names in the MediaMonkey "album artist" as the Kodi "artist".
 musicvideo_artist_albumartist_nfo.dat uses artist names in both the MediaMonkey "artist" and "album artist" as the Kodi "artist"
 
 Once you have loaded a configuration file you are set.  Click the "OK" button in the dialog and your nfo wiles will be created.
 An info popup will ask if you want to display report.  Click "No".

That's it.  .nfo files will be created for every selected music video file, placed along side it.  Note that you must use the 
MediaMonkey standard "; " item separator in your MediaMonkey library.  The script will convert these to " / " which
is the Kodi standard.  The file will be written in UTF-8 encoding, so your Unicode tags should be copied correctly.

After you load the configuration file, it will saved to your MediaMonkey settings file so you don't need to load it again.

Credit:

This script is based on the "CreateReport" script developed for MediaMonkey by trixmoto.  The original script (and many 
other useful scripts) are available at http://trixmoto.net  Thanks to trixmoto for permission to use his work.

   