# Git

Git is a tool used by developers to keep a record of changes made to code files. As you go about the business of writing
code, you will find yourself making changes all the time. You could just save a file containing the version of the code
you wrote. Then you could arrange the versions you saved in its own directory, then you could go look for that
particular file that contains the version you want to look at. If, by some chance, you forgot what version you needed,
you could just go through the directory and look at every file you have.

Or you could just use Git. Git is a version control tool. It will keep track of every change in every file you work
with. It can also keep a log of what changes you made and when you made them. You can go back to any version of any file
you need easily. There are *a lot* of things you can do with Git to keep track of the development of your project. In
this section we will get you started with using Git.

## `git`

The program that you will use is called `git` (rhymes with "sit"). It is the command-line tool that you will be using to
make "snapshots" (called "commits") of your changes.

## GitHub

GitHub (<https://github.com>) is a website that allows developers to share their code with each other. Developers can
make changes in different files and share those changes with others through GitHub.

## Git and GitHub are Not the Same Thing

Git and GitHub are not the same tools. Git is for tracking changes made in your files. These files can be anything you
want, they don't have to be code files. Once you apply Git to your project, it will keep track of changes made to your
files as you make them. The terms `Git` and `Github` are often used interchangably online. This is not correct.
`Git` is a version control tool. `GitHub` uses `Git` to make collaborating with other people possible. It is, perhaps,
unfortunate that the name `GitHub` was chosen for the website.
It can be very confusing.

You can use Git without using GitHub. But if you want to collaborate with others on a project, you'll want to use
GitHub. You can use GitHub through their GUI on the website or you can use Git and GitHub from the command line in the
terminal. We will discuss more about GitHub in future modules. For now, let's get comfortable using just Git.
Once you understand how Git works, learning GitHub will be much easier.

## Terms

Before we get started, let's define some terms.

* `Repository`
    - A central location in which data is stored and managed

* `Working Directory`
    - This is the directory your are doing the work in.

* `Head`
    - This is the latest version of a file saved to the repository.

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
