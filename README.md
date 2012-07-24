Sublime-Text-2-Syntax-Coloring-for-Visual-FoxPro
================================================

See this link for for a screenshot: http://bit.ly/M0Ic48

This is an early version of the syntax coloring file, but it's working pretty well for most PRG files that I've worked with so far.

## About the files...
There are 2 files in this repo. One is the JSON source that you use to define the coloring patterns, and then you do a "build" that file to generate the actual XML file that Sublime Text 2 uses to do the coloring.

>JSON Source file: Visual Foxpro.JSON-tmLanguage  
 XML file: Visual Foxpro.tmLanguage  

Technically, you only need the XML file to allow Sublime Text to do the coloring. If you want to make changes you could hack the XML directly, but it's a better practice , to edit the JSON file, and then do a "build" to re-generate the xml file.

##Where to place the files...
Copy the files to this location (Windows 7 folor location):  
>"C:\Users\<<UserName>>\AppData\Roaming\Sublime Text 2\Packages\User\"
