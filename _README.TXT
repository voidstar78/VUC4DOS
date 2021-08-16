12345678901234567890123456789012345678901234567890123456789012345678901234567890
         1         2         3         4         5         6         7         8

VOIDSTAR'S UTILITY COLLECTION
-----------------------------
PREPARED  August  12th,  2021

The following are a collection of programs I wrote in the early 1990s.  The 
source code for these programs were destroyed in my first (and only) complete 
hard drive crash that happened around 1995.   Often some files can be recovered
in such a crash, but in this case, it was a total lost.  It hurt, I cried,
but the world didn't end.

I also lost all the config and user data files for my BBS (originally named The
Lost Cities, later renamed to COTU - Center of the Universe).  But by the 
mid-1990s, dial-up internet was becoming available in my area (North Florida),
effectively replacing the need for any single-connection BBS.

All of these utilities were likely written in some version of Turbo Pascal.

To avoid any doubt on the matter: I officially release all of these 
executables to the Public Domain. All the original source code to these 
projects have long been lost.

Before my infamous hard drive crash, I was striving to build up my own software
development shop.  I started with the name High Magic Software, and later
changed to Provident Software (to sound more mature).  These are likely not 
the most recent build of these programs, they were older backups that we 
happened to find in my old closest on 3.5" disks around 2019.  That said, 
some of them may still be useful, but there is no way to easily correct or 
modify any of them with no source code being available.  (the spellings 
errors in CDIR could probably be corrected with a HexEditor though).

If you have any question, try the following contacts:

contact.steve.usa@gmail.com
lewissa78@gmail.com

I may end up not checking those often, so don't feel like you're ignored if
no immediate response.   But as alternatives:  I'm not really big on social 
media like Twitter, FB.  As a non-gmail way to try to contact me, maybe seek 
me from one of the YouTube videos:

https://www.youtube.com/watch?v=yotJNz-jlDQ

I am also the author of Destiny Hunter (originally for the Commodore PET,
but there is also an IBM PC port):

https://destinyhunter.org/
https://github.com/voidstar78/DestinyHunter


Cheers and Happy Vintage Computing,

v*


12345678901234567890123456789012345678901234567890123456789012345678901234567890
         1         2         3         4         5         6         7         8


PROGRAM         SIZE/DATE   DESCRIPTION
=============   =========
2ARJ.EXE          9K/????   Convert ZIP2ARJ  |works by invoking SHELL commands to PKZIP and ARJ
ADDZIP.EXE        6K/1991   Add ZIP Comment  |works by invoking PKZIP -C, can search wildcards and uses provided file as the comment

ANSMACRO.EXE      6K/1991   ANSI Macro       |uses ANSI.SYS to define keyboard macros
MACRO.KEY                                    |support file for ANSMACRO.EXE
MACRO.LST                                    |support file for ANSMACRO.EXE

ASK.EXE	         10K/???? * Ask User         |used in scripts to ask a question and then uses ERRORLEVEL to determine the response to the question
ASKDEMO.BAT                                  |an example of how to use the ASK.EXE errorlevel results

CARRIER.EXE       6K/1992   Carrier Detect   |examines COM port to see if a carrier is present, returns different ERRORLEVEL if so (requires a FOSSIL.SYS driver)
CDIR.EXE	 15K/1995 * ColorDIR 3.1b    |use “cdir ?” because “cdir -h” seems to causes lockup
CDIR30.EXE	 11K/1991   ColorDIR 3.0     |funny “cdir -h”, can run out of memory if there is a large number of files in the folder
CHATTRIB.EXE	 20K/1991   ChangeAttributes |really just my intro to Pascal and using the OPRO GUI library
CLOCK.EXE	  9K/1991   Clock In/Out     |writes current time to a specified command line filename, I used it to track my time at my first job
DELALL.EXE        7K/1991   DeleteAllFiles   |delete all files of a given wildcard; typically I used this to remove extra FILEID.DIZ
DELSIZE.EXE       7K/1991   DeleteSize       |delete files of a specified byte size; typically I used this to remove 0 byte files
EDIT.EXE	 31K/1991   TextEditor       |I believe this is a real-mode program and limited to editing files no longer than 64KB	
FILELIST.EXE     15K/????   Make FileList    |Scan a directoy structure and list all the files in specified output file (e.g. FILELIST.TXT
MR.EXE	         10K/???? * Memory View	     |shows what is current consuming system memory; I had a newer version that also reported CPU type, was similar to CheckIt
NUKE.EXE	  7K/1990 * Nuke 1.0	     |nuke all contents of a specified folder and recursively remove all subfolders)  (safe to run with no command line arguments
PHONE.EXE	 22K/1992   Phone Database   |a later demo of using the OPRO library for a simple database entry system; a later version included the ability to attach and preview TIF images with entries
QMATH.EXE	  7K/???? * QuickMath        |command line math calculator, like "qmath 5.2+(4.8-3.5)*2"
REBOOT.EXE	  3K/???? * Reboot the Systme from Command Line
SEARCH.EXE        6K/???? * Search for File  |wildcards supported, recursively search specified folder; provides summary of total bytes used by all the found files
TERMINAL.EXE	 11K/1991   (Simple) Terminal|my first attempt at a simple terminal connection program, and included Zmodem support
TEXTATTR.EXE	  4K/1990 * Show all IBM PC text attributes|help remind what code is what effect
TIMEIS.EXE        5K/????   What Time Is It  |writes the current time and date to DOS screen in plain-text, but this output cannot be pipped to a file
TSAR.EXE	  7K/1992   Text Search and Replace|scan a text file and replace content based on command line arguments
XMIT.EXE	  5K/????   Xmit Time        |estimates file transfer times using command line arguments

* - This is to mark which utilities that I believe are the most useful
    and functionally complete.  If one is using floppies only, and space
    is limited, then the "*" set of tools are probably a good candidate
    for a "minimal distribution."  This is a subjective selection based
    on my own opinion (I included TEXTATTR in the list just as a good
    demo/sample program for CGAs; but things like XMIT, TSAR, TERMINAL,
    are all useful too - obviously be careful with NUKE, DELALL, DELSIZE;
    I consider 2ARJ and ADDZIP essentially useless since they are just
    SHELL wrappers - i.e. they depend on other tools to be present, but
    they exist as my introduction project into Pascal and the MS-DOS
    environment).

							

OTHER NOTES
===========
QMATH.EXE - I think I integrated a math expression parser that may have been included with Borland Pascal.

EDIT.EXE - I recall finding an older source code to an editor that was very broken, so I modernized it and added various new features.

ASK.EXE/REBOOT.EXE - not sure if these were mine or not (I recall reading up on how to make a program like these, but these might actually be earlier copied that inspired me)

CDIR - very much mine, and in the HELP notes of CDIR30 I am reminded I was inspired by the original HDIR.COM (HotDir) from several years earlier
   NOTE: my later advanced version of CDIR would save preferences by writing directly into the EXE itself (e.g. to adjust color preferences for file types).


OTHER PROJECTS (all lost in the crash)
==============
Katinator    (graphical adventure)
DOS-Boss     (file manager, pre Windows 3.X)
TankGame     (networked game with tank combat)
Exploration  (a text-graphics clone of Sid's Civilization)
Xiphod BBS   (my personal branch of Forum BBS source)

...and dozens of other various utilities...

