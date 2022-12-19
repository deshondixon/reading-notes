# Practice in Terminal

## *The Command Line*

I have a pretty good understand of the command line from previous classes.

A command line, or terminal, is a text based interface to the system. You are able to enter commands by typing them on the keyboard and feedback will be given to you similarly as text.

Opening a terminal is fairly easy. I can't tell you exactly how to do it as every system is different but here are a few places to start looking.

If you're on a Mac then you'll find the program Terminal under Applications -> Utilities.

An easy way to get to it is the key combination 'command + space' which will bring up Spotlight, then start typing Terminal and it will soon show up.

If on Linux then you will probably find it in Applications -> System or Applications -> Utilities. Alternatively you may be able to 'right-click' on the desktop and there may be an option 'Open in terminal'.

If you are on Windows and intend to remotely log into another machine then you will need an SSH client. A rather good one is Putty (free) .

-------------------------------------------------------------

## *Basic Navigation*

I know how to navigate in the terminal fairly well so nothing from this section was new to me.

The first command we are going to learn is pwd which stands for Print Working Directory. (You'll find that a lot of commands in linux are named as an abbreviation of a word or words describing them. This makes it easier to remember them.) The command does just that. It tells you what your current or present working directory is

It's one thing to know where we are. Next we'll want to know what is there. The command for this task is ls. It's short for list. Let's give it a go.

In order to move around in the system we use a command called cd which stands for change directory.

pwd

Print Working Directory - ie. Where are we currently.

ls

List the contents of a directory.

cd

Change Directories - ie. move to another directory.

-------------------------------------------------------------

## *More About Files*

Ok, the first thing we need to appreciate with linux is that under the hood, everything is actually a file. A text file is a file, a directory is a file, your keyboard is a file (one that the system reads from only), your monitor is a file (one that the system writes to only) etc. To begin with, this won't affect what we do too much but keep it in mind as it helps with understanding the behavior of Linux as we manage files and directories.

This one can sometimes be hard to get your head around but as you work through the sections it will start to make more sense. A file extension is normally a set of 2 - 4 characters after a full stop at the end of a file, which denotes what type of file it is. The following are common extensions:

file.exe - an executable file, or program.

file.txt - a plain text file.

file.png, file.gif, file.jpg - an image.

Linux actually has a very simple and elegant mechanism for specifying that a file or directory is hidden. If the file or directory's name begins with a . (full stop) then it is considered to be hidden. You don't even need a special command or action to make a file hidden. Files and directories may be hidden for a variety of reasons. Configuration files for a particular user (which are normally stored in their home directory) are hidden for instance so that they don't get in the way of the user doing their everyday tasks.

To make a file or directory hidden all you need to do is create the file or directory with it's name beginning with a . or rename it to be as such. Likewise you may rename a hidden file to remove the . and it will become unhidden. The command ls which we have seen in the previous section will not list hidden files and directories by default. We may modify it by including the command line option -a so that it does show hidden files and directories.

-------------------------------------------------------------

## *Manual Pages*

The manual pages are a set of pages that explain every command available on your system including what they do, the specifics of how you run them and what command line arguments they accept. Some of them are a little hard to get your head around but they are fairly consistent in their structure so once you get the hang of it it's not too bad.

It is possible to do a keyword search on the Manual pages. This can be helpful if you're not quite sure of what command you may want to use but you know what you want to achieve. To be effective with this approach, you may need a few goes. It is not uncommon to find that a particular word exists in many manual pages.

-------------------------------------------------------------

## *File Manipulation*

Linux organizes it's file system in a hierarchical way. Over time you'll tend to build up a fair amount of data (storage capacities are always increasing). It's important that we create a directory structure that will help us organize that data in a manageable way. I've seen way too many people just dump everything directly at the base of their home directory and waste a lot of their time trying to find what they are after amongst 100's (or even 1000's) of other files. Develop the habit of organizing your stuff into an elegant file structure now and you will thank yourself for years to come.

Creating a directory is pretty easy. Removing or deleting a directory is easy too. One thing to note, however, is that there is no undo when it comes to the command line on Linux (Linux GUI desktop environments typically do provide an undo feature but the command line does not). Just be careful with what you do. The command to remove a directory is rmdir, short for remove directory.

-------------------------------------------------------------

# *Cheat Sheet*

## Basic Navigation

pwd
Where am I in the system.

ls [path]
Perform a listing of the given path or your current directory.
Common options: -l, -h, -a

cd [path]
Change into the given path or into your home directory.

Path
A description of where a file or directory is on the filesystem.

Absolute Path
One beginning from the root of the file system (eg. /etc/sysconfig ).

Relative Path
One relative to where you currently are in the system (eg. Documents/music ).

~ (tilde)
Used in paths as a reference to your home directory (eg. ~/Documents ).

. (dot)
Used in paths as a reference to your current directory (eg. ./bin ).

.. (dot dot)
Used in paths as a reference to your current directories parent directory (eg. ../bin ).

TAB completion
Start typing and press TAB. The system will auto complete the path. Press TAB twice and it will show you your alternatives.

-------------------------------------------------------------

## More About Files

file [path]
Find out what type of item a file or directory is.

Spaces in names
Put whole path in quotes ( " ) or a backslash ( \ ) in front of spaces.

Hidden files and directories
A name beginning with a . (dot) is considered hidden.

-------------------------------------------------------------

## Manual Pages

### *Ignore quotes*

man (<)command(>)
View the man page for a command.

-------------------------------------------------------------

man -k (<)search term(>)

Search for man pages containing the search term.

-------------------------------------------------------------

Press q to exit man pages

-------------------------------------------------------------

## File Manipulation

### *Ignore quotes*

mkdir (<)directory name(>)

Create a directory

-------------------------------------------------------------

rmdir (<)directory name(>)

Remove a directory (only if empty).

-------------------------------------------------------------

touch (<)file name(>)

Create a blank file.

-------------------------------------------------------------

cp (<)source(>) (<)destination(>)

Copy the source file to the destination.

-------------------------------------------------------------

mv (<)source(>) (<)destination(>)

Move the source file to the destination.

May also be used to rename files or directories.

-------------------------------------------------------------

rm (<)path(>)

Remove a file or directory.

Common options: -r -f

-------------------------------------------------------------

# *References*

<https://ryanstutorials.net/linuxtutorial/>

<https://ryanstutorials.net/linuxtutorial/commandline.php>

<https://ryanstutorials.net/linuxtutorial/navigation.php>

<https://ryanstutorials.net/linuxtutorial/aboutfiles.php>

<https://ryanstutorials.net/linuxtutorial/manual.php>

<https://ryanstutorials.net/linuxtutorial/filemanipulation.php>

<https://ryanstutorials.net/linuxtutorial/cheatsheet.php>
