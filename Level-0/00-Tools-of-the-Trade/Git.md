# Git

Git is a tool used by developers to keep a record of changes made to code files. As you go about the business of writing
code, you will find yourself making changes all the time. You could just save a file containing the version of the code
you wrote. Then you could arrange the versions you saved in its own directory, then you could go look for that
particular file that contains the version you want to look at. If, by some chance, you forgot what version you needed,
you could just go through the directory and look at every file you have.

Or you could just use Git. Git is a version control tool. It will keep track of every change in every file you work
with. It can also keep a log of what changes you made and when you made them. You can go back to any version of any file
you need easily. There are *a lot* of things you can do with Git to keep track of the development of your project. In
this section we will get you started with using Git and GitHub.

## `git`

The program that you will use is called `git` (rhymes with "sit"). It is the command-line tool that you will be using to
make "snapshots" (called "commits") of your changes.

## GitHub

GitHub (<https://github.com>) is a website that allows developers to share their code with each other. Developers can
make changes in different files and share those changes with others through GitHub.

## Git and GitHub are Not the Same Thing

Git and GitHub are not the same tools. Git is for tracking changes made in your files. These files can be anything you
want, they don't have to be code files. Once you apply Git to your project, it will keep track of changes made to your
files as you make them.

You can use Git without using GitHub. But if you want to collaborate with others on a project, you'll want to use
GitHub. You can use GitHub through their GUI on the website or you can use Git and GitHub the command line in the
terminal. We will be using the command line.

## Terms

Before we get started, let's define some terms.

* `Repository`
    - A central location in which data is stored and managed

* `Clone`
    - And exact copy of a repository stored on your machine. When you clone a repository two identical copies of the
      repo exist, one on your machine and one stored in a GitHub account (online).

* `Fork`
    - When you make an exact copy of a repository from another GitHub account into your own account, you have created
      a fork. This is the same as a clone. The difference is clones are copies made on your machine from a GitHub
      account. Forks are copies made from one account to another account. This is a common action to do on GitHub. It
      allows developers to share files for a wide variety of different projects. Often, developers will invite other
      developers to work on their code.

* `Remote`
    - This is the repository stored in the GitHub account.

* `Local`
    - This is the copy of the repo stored on your machine.

* `Head`
    - This is the latest version of a file saved to the repository.

* `Origin`
    - This is the word used to refer to the repository from which your clone was made.

How does this all work? Think of Git as a time line. Changes you make are saved and placed on this time line. As you
move forward, every change you save is recorded on this line. The last (most recent) saved change you made is the *head*
of the timeline. The next change you make will be compared to HEAD then added as the new HEAD. This continues until
there are no more changes you wish to make.

How do I collaborate with other developers? Different developers can work together on the same code by using a GitHub
feature called "branching". Instead of just moving forward with new versions always becoming HEAD, you can divert off
the main timeline and create a parallel timeline. This is a "branch". Here you can work on your code without affecting
the work already done on the main timeline. This main timeline is called the "master" branch. When you are finished with
your changes, you can merge your branch back into the master branch. GitHub will automatically sort everything on both
branches to make it all align.

Let's get you working with Git and GitHub.

* Navigate over to the GitHub website. Create an account for yourself. (We will need that later)

* Open a terminal window on your machine (CTRL+ALT+t)

* Navigate to your Projects directory. (If you don't have a Projects directory, make one with `mkdir Projects`).

* Type `git init`. This command creates a git repository.

* Type `git status`. This will show you the current state of your repo. It will show you what files are tracked (or
  not tracked), what files have been changed, and what has been staged. What does all that mean, exactly? Let's go over
  that now:

    - There are three steps to saving a file to your repo.

    - First, you make changes in a file or in several files. Git tracks every file you have changed.

    - If you satisfied with the changes you have made, you add the files to the staging area with the command
    `git add [the filename of the file you want to add]`.

    - To permanently save your files to your repo type `git commit -m "A short summary of the work done"`. Use quotes for
    the message part.

    - Once you committed your file, that's the end of the cycle. You can always make additional changes later and then add,
    stage, and commit them as well. In fact, it is expected that you do.

The above is the basic set of steps used to create a repository, add files to the staging area, and commit (permanently
save) them to your repo.

## Getting to the Repository

In the previous section we went over how to create a repository on your machine, and then making changes and saving
them. This is fine for tracking your own files, but how do you get into a repository that is being used by other
developers? This is when you will need to clone the repo.

When you clone a repo you are making a complete copy of the repository stored on your machine. Any changes you make in
the cloned repository exist only in the clone. They do not change anything in the repository you made a clone from.
Let's look at how to clone a repository onto your machine.

* Open a terminal window and navigate to the directory you want to store your clone in.

* Type `git clone https://github.com/name-of-the-repository/name-of-the-repository`. This creates a copy of the
  repository on your machine.

* The repository lives in the directory you were in when you cloned it.

## Tranferring Your Data

A repository is a central location where all of the files and directories for a project are stored. When you clone a
repository, GitHub is aware that a clone has been made. It will allow you to send and receive data to the central
server (called a "remote" ).
