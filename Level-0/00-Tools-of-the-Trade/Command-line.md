# The Command Line

A long time ago there was no such thing as a mouse or a window or any other way to interact with a computer except a
keyboard and a screen. Instructions were written with the keyboard, and
output from those instructuions were viewed on the screen. That's it. There were no fancy buttons to click, no pictures,
pretty windows. It was just text and a keyboard. A user interacted directly with the computers CPU to tell it what to do.
While this seems very primitive and difficult, it turns out that some things are better done using this method as opposed to
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
of a terminal is still with us. It is no longer a physical object, but we still use a thing called a terminal. These days the
terminal is a program on your computer that mimics a real terminal. It is referred to as a "terminal emulator". An emulator
is a computer program that pretends to be something that it isn't. There are lots of different types of emulators. They all do
the same thing, they "emulate" a device or computer platform that is not physically present. We use the terminal emulator
program to create a virtual terminal on the computer. You will see this term "virtual" a lot. It means a device or program that
is recreated digitally and not the thing itself. A virtual terminal is a terminal that does everything a real terminal does,
but isn't actually a real, physical terminal object.

### Where is the Terminal?

Most computer operating systems have terminals emulators built into them. In Linux, you can open a terminal window by
pressing CTRL-ALT-t. A window will pop up with a prompt and nothing else. This is the terminal window. You will often hear
the term "open a terminal" or "open a terminal window". This is the same thing as pressing CTRL-ALT-t. In the terminal you
can do anything you would normally do by pointing and clicking a mouse.

 DRILL: Open a terminal window on your desktop

### Terminal Commands

As noted previously, commands in the terminal are really programs that you run to make things happen. This fact leads us to our
first command. Whenever you wish to run a program, *any* program, from the command line all you need to do is just type the
name of the program and press enter. This tells the shell to run that program. If the name you typed is not a program the
shell will give you the message "command not found".  Typing the name of the program and pressing Enter is how you make a
program run. Because command line commands are really programs that need to be run in order to do something they are typed
first on the line.

### Common Command Line Commands

There are *a lot* of Command Line commands. To begin we will introduce you to some of the most used commands (programs) in
the terminal. They are listed below:

* `cd`
    - This program changes the directory you are in. It is the same thing as clicking on a folder.  