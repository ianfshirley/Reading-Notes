#Command Line Tutorial Notes

### The Command Line

- I didn't know that the "-m" that I've been using when committing changes was called an Option, but I did know it's used to modify the arguments that follow (also didn't know they were called command line "arguments")
- I learned that zsh, which I have on my mac, is built on top of bash, so it has all the functionality of bash plus some add-ons

### Basic Navigation

- I already knew "ls" lists the contents of the current directory, but I didn't know how to modify with options.
- ls -l runs a long listing, with more info about each file or folder in the directory, including whether it's file or folder, the owner, file size & time it was last modified
- I don't understand what /etc does, it's not explained well. It says it does not list the current directory but instead lists that directory's contents, but that's already what "ls" does. I ran ls /etc in my terminal and I have no idea what I'm looking at.
- Absolute vs. Relative Paths:
  - Absolute paths specify a location in relation to the root directory. Relative paths specify a location in relation to the current directory.
- I didn't know you could use the "~" to refer to the home directory. That will help with navigating to directories that several levels away from the current directory.

### More About Files

- Everything is a file (files, text, directories etc.)
- Linux is an extensionless system (no need for the .exe, .txt. .png etc. after the file name)
- Linux is case sensitive
- Spaces in file names can be accounted for in two ways. You can either put the whole file name in quotes, or you can put a backslash before the space to negate the special meaning of the character that follows the backslash (in this case the space)
- As we learned in 201, there are hidden files that do not show up when you run the "ls" command, but they can be shown by running "ls -a"

### Manual Pages

- Running "man" before a command, will give you a manual regarding that command. It explains what that command does, what modifying options you can use, and which arguments you can use.
- You can also search by keyword. "man -k" and your search term will find all the manual pages that contain your search term
- Within a manual page, you can type "/" and a term/word and it will highlight all instances of that term/word within the manual page. You can type "n" to move to the next highlighted instance.

### File Manipulation

- mkdir [options] <Directory> makes a new directory.
- You can add a file path before the directory name if you want to create the directory somewhere other than the current directory.
- mkdir -p will create the directory and parent directories as needed
- rmdir [options] <Directory> removes a directory. It can be modified in the same ways as mkdir
- touch [options] <filename> creates a blank file.
- cp [options] <source> <destination> copies a file or directory.
- mv [options] <source> <destination> moves a file or directory.
- mv can also be used to rename a directory, either while moving it to a new location or keeping it in the same location and just changing the name
- rm [options] <file> removes files and directories that are not empty. "rm" by itself will just tell you that the directory you're trying to remove is a directory. "rm -r" will remove the directory.

### Cheat Sheet

- There's a helpful cheat sheet with all the terms from the tutorials. I've bookmarked it in my Code Fellows bookmarks folder.
[Linux Tutorial - Cheat Sheet](https://ryanstutorials.net/linuxtutorial/cheatsheet.php)