# The Command Line

A long time ago there was no such thing as a mouse or a window or any other way to interact with a computer except a
keyboard and a screen. Instructions were written with the keyboard, and
output from those instructuions were viewed on the screen. That's it. There were no fancy buttons to click, no pictures,
pretty windows. It was just text and a keyboard. A user interacted directly with the computers CPU to tell it what to do.
While this seems very primitive and difficult, it turns out
that some things are better done using this method as opposed to
the Graphic User Interface. We will be using the Command Line for many of the tasks associated with your work.

## The Shell

In order to communicate with the Central Processing Unit of a computer there must be a means for the computer to accept user
input and translate it into instructions the computer understands. The program used to do this is called a shell. There are
many different shells. They all pretty much do the same thing, but each one a little differently. We will be using the
BASH Shell. BASH is an acronym that means the Bourne Again Shell. It is a shell program written by Steve Bourne that
improves upon the original shell program from way back when. The acronym is an attempt at programmer humor.
How successful it is I leave to your better judgement. It is a good place to start learning the command line.
As you become more comfortable with using the command line, you may wish to use a different shell program. That's fine.
For now, we'll go with BASH.

## The Unix Philosophy

Unix is an operating system (the system that controls all of the functions of your computer). It was developed at Bell Labs
back in the 1970's. The Linux Operating System is based on this early operating system. The philosophy of Unix was to
utilize small programs written to execute specific tasks. When you give a "command" in the shell, you are really running
a program to execute a task. Understanding this idea makes learning the command line a lot easier. Each "command" is a program
that does a something. Linux operates in the same way. Everything from moving a file to establishing an internet connection
is done by executing a program that does one thing. Then you might execute another program that does *another* thing.
Inputs and outputs of these programs can be directed in various ways. By utilizing a series of programs and directing the
input and output as needed, tasks get done. All of this may sound complicated, but actually it can make things a lot easier
and faster. Let's get started using the command line.

## The Terminal

A terminal is a device used to enter data into and extract data from a computer. You could think of it as an access point
between the computer and the user. Long ago, the only way to interact with a computer was to feed it cards or lengths of
paper tape imprinted with instructions. The computer would execute the instructions then print the result on a card or paper
tape. At that time, terminals did exist, but were much slower than using cards or paper tapes. As time went on, terminals
began to perform better and better. Eventually, they became the primary means of interacting with the computer. It must be
born in mind that at this time computers were still giant machines costing tens of thousands of dollars. A terminal was
connected to the computer in order to interact with it. There was little if any computing power in the terminal unit itself.
It was just a communication portal to the computer. Later, terminals were developed with varying degrees of computing capabilities.
However, they still relied on a main computer often located somewhere else than the location of the terminal.
Several terminals would be connected to the same computer. This was standard practice until the advent of micro computers
(That's the kind of computer you are looking at right now.) Fascinating history lesson , but so what, right? Well, the idea
of a terminal is still with us. It is no longer a physical object, but we still use a thing called a terminal.
These days the
terminal is a program on your computer that mimics a real terminal.
It is referred to as a "terminal emulator". An emulator
is a computer program that pretends to be something that it isn't.
There are lots of different types of emulators. They all do
the same thing, they "emulate" a device or computer platform that is not physically present.
We use the terminal emulator
program to create a virtual terminal on the computer. You will see this term "virtual" a lot.
It means a device or program that
is recreated digitally and not the thing itself.
A virtual terminal is a terminal that does everything a real terminal does,
but isn't actually a real, physical terminal object.

### Where is the Terminal?

Most computer operating systems have terminals emulators built into them.
In Linux Ubuntu, you can open a terminal window by
pressing CTRL-ALT-t. A window will pop up with a prompt and nothing else. This is the terminal window. You will often hear
the term "open a terminal" or "open a terminal window". This is the same thing as pressing CTRL-ALT-t. In the terminal you
can do anything you would normally do by pointing and clicking a mouse.

DRILL: Open a terminal window on your desktop

### Terminal Commands

As noted previously, commands in the terminal are really programs that you run to make things happen.
This fact leads us to our
first command. Whenever you wish to run a program, *any* program, from the command line all you need to do is just type the
name of the program and press enter. This tells the shell to run that program. If the name you typed is not a program the
shell will give you the message "command not found".  Typing the name of the program and pressing Enter is how you make a
program run. Because command line commands are really programs that need to be run in order to do something they are typed
first on the line.

### The Directory Tree

The files and directories (often incorrectly called a folder) on your computer are organized in a specfic way.
This organization is referred to as a "tree".
At the top of the tree there is a single folder called "root". Inside this directory are other directories that in turn
contain yet more directories. Inside most of these directories there are individual files.
If you lay it all out on paper, the file system looks like an upside down tree. By using this system of organization your
computer can keep track of where all of your data is at any given moment.
This system of file organization is very common throughout many programs and applications, not just in the terminal.
It is a good idea to get familiar with it as you will be using it in many different places in your development process.

### How Do I Find My Data?

In the previous section we talked about the organizational structure of the file system.
You can think of this structure as a
series of roads.
In order to arrive at the directory that contains your data, you have to travel a road.
This road is called a file path.
Every file on your computer lives inside of a directory somewhere.
You must lay out the road starting with where you are and
ending with where you want to go. This is always going to be from one directory to another directory
(Remember, every file lives in a directory). Here is an example of a typical file path: `Home/Projects/dev-training/my-addresses.txt`.
You can see here we started at a directory called Home then proceeded through two more directories(Projects and dev-training)
to arrive at the my-addresses.txt file.
But why did we need to go through two additional directories to get to the file we wanted?
Ok, so while we call the file system a tree, it's actually clusters of directories inside other directories.
Inside those directories are files. You could take the above file path and translate as "In the Home directory there lives
the Project directory.
Inside the Projects directory there lives the dev-training directory.
Inside this directory there lives the file my-addresses.txt. Let's go there please." Placing things inside other things is
called "nesting". This idea is very prevalent in software development.
The tree file structure is really a nested directory structure.
If you spread it all out, it does look like an upside down tree, but you can also think of it as things inside of things.
Most of the time it will be referred to by the tree analogy, so you should probably go with that.

#### Relative and Absolute File Paths

An absolute file path is one that specifies the path starting from the root directory(The first directory there is). If you
use an absolute file path you can go anywhere you want to go without having to worry about
which directory you are currently in. You can only do this if you specify the entire file path starting from the root directory.
Sometimes that can get pretty long. If you don't want to write out the whole path, you can use a relative file path. A
relative file path is a path that is relative to the directory you are in.
That means starting from the directory you are in then going forward from there. Using this file path

### Common Command Line Commands

As mentioned before, command line commands are actually programs that are run in order to do something.
There are literally thousands of different commands you can use. No one could possibly remember all of them.
And more are being created all the time.
So, how do you know what to use and how to use it? Every command line command has a help section and a manual.
You can access these by typing either `[command] help` or `man [command]`. That last one is short for "manual".
It will tell you everything you need to know about that particular command.
Bear in mind that sometimes there is quite a lot of material covered in the help or man pages. Don't be discouraged by this.
Remember, no one knows it all. Google is your friend. Use it to ask questions.
There are thousands of different resources on the internet. You will definitely find the answer...eventually.
As you become more familiar with your tools and their use, your ability to
quickly find the data you are looking for will improve.

#### Command Line Arguments

Command line programs can be "tweaked" in order to specify exactly how you want them to run. This is done by specifying the tweak
(more properly called an "argument") after writing the command itself. It would look something like this: `ls -la`.
This command says, "List out the contents of this directory, and I want the long version (l) and I want everything,
including anything hidden (a)." You might have noticed the arguments are preceeded by a "-".
You can use this or you can use "--".
This second double dash is used when you want to write out the whole argument. So, you could say "-v" for version, or you
could write "--version". Both of these arguments do the exact same thing.

* `pwd`
    - This command tells you which directory you are currently in. If you get lost this command helps you get unlost.

* `cd`
    - This command moves you around to
    different directories. You can use either a relative file path or an absolute file path.
    If you use the absolute file path it doesn't matter what directory you are currently in. If you use a relative file path,
    you must designate the file path relative to the directory you are currently in. If you just type `cd` with no file path,
    you will be taken to your home directory

* `ls`
    - This command lists the contents of the directory you are currently in. If you want to see the contents of a different
    directory, type `ls` followed by the directories path.
    `ls/home/username/Documents` will show you the contents of the Documents directory.

* `cat`

    - This command is short for "concatenate". It lists the contents of a file. To use it, type `cat name-of-file.file-extension`.
    This will allow you to view the contents of the file, but it does not allow for editing.

* `cp`

    - This is the copy command. If you want to copy a file into a directory, you would write it like this:
    `cp my-file.txt my-directory`. In this example, "my-file.txt" is the filename and "my-directory" is the name of the directory.
    This tells the computer to make a copy of the file and place that copy in the directory you specified in the command.
    Once the command is executed, there will be two copies of the file.
    One is the original file and the other is the same(copied) file located in the directory you specified in the command.
    Remember, you must specify the file path to the directory where
    you want your copied file to go.

* `mv`

    - This command is short for "move". It is used to move files around, but it can also be used to rename a file.
    This can be a little confusing.
    How does moving a file relate to renaming a file? Let's take a look at it.
    Files can only be moved into a directory. So,
    if you type `mv my-file.txt my-directory` you are telling the computer to move "my-file.txt" into the "my-directory"
    directory. Moving a file is very similar to making a copy,
    but instead of making a copy and placing it into a directory you have
    moved an already existing file into a directory.
    If you wanted to rename a file instead of moving it, you would write the
    same command, except instead of specifying a directory you would supply a new file name. it would look like this:
    `mv my-file.txt your-file.txt`. This command changes the name of the file "my-file.txt" to "your-file.txt".

* `touch`

    - To create a new file use the `touch` command. The command looks like this: `touch new-file.txt`.
    This creates the file in the current working directory (The one you are currently in). If you want to create a new file
    and put it somewhere other than the current directory you must specify the file path.
    In this case it would be an absolute file path. It would look like this: `touch /home/username/Documents/my-file.txt`.
    This will create a new file located in the Documents directory.

* `mkdir`

    - When you want to create a new directory, you use this command. It looks like this: `mkdir My-Directory`.
    This will create a directory in the current working directory.
    If you want to make a directory someplace else, you must specify the file path.
    This command has a tweak (argument). It's `-p`. It means "parent".
    When you use this argument you can create a series of
    directories nested inside each other. It would look something like this: `mkdir -p Foo/Soo/Boo`. This creates a directory
    called "Foo". Inside that directory there lives the directory "Soo".
    Inside the Soo directory there lives the "Boo" directory.
    If the directory does not already exist, one will automatically be created.

* `rmdir`

    - If you need to remove a directory, use this command. It will only remove directories that are empty.
    The directory you want to remove can't have any other directories or files in it at the time you want to remove it.

* `rm`

    - This command removes a *file* from a directory. It will not remove a directory, just the file. However,
    if you use the `-r` argument and type in a directory name, it will delete the directory *and everything in it*.
    It would look like this: `rm -r directory-name`. Be careful with this command.
    There is no fetching the directory from a trash can. Once it is gone, *it is gone forever*.

* `touch`

    - This command creates a new file. If you need a new, empty file use `touch`.
    You have to say what you want the name of the file to be.
    It looks like this: `touch filename` . Using a absolute file path, you can specify where you want your file created.
    That would look like this: `touch /home/username/Documents/new-file.txt` . This command will create a new file
    called `new-file.txt` inside the Documents directory. Bash doesn't care about file extensions.
    It just reads whatever you wrote there.
    However, we humans *do* care about file extensions. They tell us what kind of file we are dealing with.
    Other programs also care about file extensions. It tells them what files belong to them and what files belong to
    something else. For example, files containing C++ code would have a file extension of `.cpp` or `.c` while a Javascript
    file would have a `.js` file extension, and so on.
    When you create your new file it is a good idea to include a file extension so you know what that file is for.
    If you create a file without a file extension it will be given a `.txt` file extension by default.
    That means its just a text file.

* `locate`

    - If you need to find a file, use the `locate` command. It looks like this: `locate name-of-file.ext` .
    But what if you don't know the exact name of the file? In that case you can use the `*` argument.
    The `*` is known as the wildcard. It means "give me anything and everything". In combination with at least one word you
    think might be in the filename, the wildcard can narrow down your search. Here is an example: `locate *.txt` .
    This tells the computer to find anything that has a `.txt` file extension.
    Granted, that particualar command doesn't really narrow down anything.
    You could also use something like this: `locate name*box` .
    This command will locate any file that has the word "name" and the word "box" in it. You can also use the `-i` argument
    to make the search case insensitive.
    What do we mean by "locate"?
    It means that the computer will return the file path to the file.
    If there are multiple matches to what you are looking for, each file path will be returned.
    If you are not specific enough, you could get several pages of file paths.
    What the command is doing, actually, is looking for the words you typed and displaying every instance where that word or
    words exist in a file path. So, it's a pretty broad search. The command will find anything you tell it.
    It helps to be as specific as you can.

* `find`

    - Similar to the `locate` command, `find` is used to find 
