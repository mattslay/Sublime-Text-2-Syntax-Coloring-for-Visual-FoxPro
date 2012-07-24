Sublime-Text-2-Syntax-Coloring-for-Visual-FoxPro
================================================

This is an early version of the syntax coloring file, but it's working pretty well for most PRG files that I've worked with so far. If you dig in and make any changes, please for this repo and send a pull request.  

See this link for for a screenshot: http://bit.ly/M0Ic48


## About the files...
There are 2 files in this repo. One is the JSON source that you use to define the coloring patterns, and then you do a "build" on that file to generate the actual XML file that Sublime Text 2 uses to do the coloring.

>JSON Source file: Visual Foxpro.JSON-tmLanguage  
 XML file: Visual Foxpro.tmLanguage  

Technically, you only need the XML file to allow Sublime Text to do the coloring. If you want to make changes you could hack the XML file directly, but it's a better practice to edit the JSON file, and then do a "build" to re-generate the xml file.

##Where to place the files...
Copy the files to this location (Windows 7 folor location):  
>"C:\Users\\<UserName\\>\AppData\Roaming\Sublime Text 2\Packages\User\"

## How to develop, build, or customize
I'm sure there is plenty of work that needs to be done on the JSON definition file to really fine tune this coloring and properly define the FoxPro language. It has the notion of "scopes", "keywords", "control structures", and so on. My guess is that properly defining each of these areas allows Sublime to carry out some of it's advanced editing features, but that's jsut a guess. I've only spent a small amount of time with it so far, but, hey, as you can see from the screen shot link above, it seems to work pretty well for now.

(Note: the current list of keywords that you'll see at the top of my JSON file is just a list I extraced from an existing NotePad++ syntax file that's been around for a few years. I have moved a few of the keywords out of this main blob and down into sepatate blocks at the bottom of the file to make it clearer and to begin the proper separation of the words by their syntax type. More work probably needs to be done in

So, if you want to dig in and get involoved, here are the steps to learn the JSON syntax for defining a language file in Sublime Text, and the steps you'll need to take to do a "build" on that JSON file to generate the working XML file that ultimately does the actual work. Hint, you've got to install a little package in Sublime to get the JSON-to-XML builder tool. You'll see instructions at the very top of this page:  
>http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/extensibility/syntaxdefs.html?highlight=syntax

## Additional resources...
If found this JSON definition file for the VB.Net langauge which helped me see the various sections of the JSON definitions that can be used to properly define the various "scopes", "keywords", "control structures" sections. I think you can get some good understanding of a language definition by studying this package:

https://github.com/angryant0007/VBDotNetSyntax/blob/master/vbdotnet.JSON-tmLanguage


