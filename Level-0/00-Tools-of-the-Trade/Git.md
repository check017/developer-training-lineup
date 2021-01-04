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

* `Working Directory`
    - This is the directory your are doing the work in.

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

How do I collaborate with other developers? It is possible to collaborate directly with another developer using only Git.
This is known as a peer-to-peer arrangement. You and someone else are connected directly to each others' machines.
You grant access to your machine and your friend grants you access to his/her computer.
In order to work on your project you
must be connected online.
With GitHub, a developer can clone a repository, work on their files, and then send those files
back to the main (remote) repository.
An internet connection is not required. When the developer is ready to send his work to
origin, he can connect to GitHub, push his code, and then disconnect.
GitHub also provides several features that allow
collaborators to effectively work together on a project.

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

Git allows developers to share their data with each other. Usually, a single member of a team will clone the repo, then
create a *branch*. A branch is an alternate timeline running parallel to the main timeline. The main timeline is called
*master*. Actually, master is a branch itself, but it is more useful to think of it as the trunk of a tree. Other branches
divert off master and move forward in time parallel to master. The value of a branch is that the changes you make have no
effect on the code tracked on the master branch. You can break things, experiment, and generally just play around with your
code without fear of breaking anything important.
The branching feature is used more than just experimenting.
A new feature being
added to an application would be developed on its own branch.
In this way, a new feature can be worked on and tested before
being added to the main body of the code.
Branching also allows for several different developers to all work on the same code
independantly. We will cover the basic actions of sending and receiving data using GitHub.
Let's cover some terms to begin with.

* `push`
    - This is the action of sending your committed files to the remote repository.

* `pull`
    - This is the action of retrieving data from remote repository.

* `fetch`
    - This is the action of checking a remote repo to see if there have been any changes.
  No files are transferred when fetching.

* `diff`
    - This command will show the changes made before and after you have made changes.
  It will also show any changes that have
  been made in the remote compared to your local repo

* `pull request`
    - This a request made to the person in charge of the repo. You are asking that your changes be approved, and if
    acceptable, that they be merged into the master branch.

* `merge`
    - When a branch is intergrated back into another branch.
      This is done when work on the branch is complete. It is then
      reintergrated into the branch from which it was created.

Keep in mind there are a lot of things Git allows you to do.
But, just to get started, we will cover the basic procedure for
working with files, saving your changes and then pushing those changes to the repo.
Let's walk through it as if you were
starting your day.

First thing is to fire up your machine. Once booted up, open a terminal window and navigate to your git repository.

We need to check to see if there have been any changes made since the last time you pulled from the repo. Type `git fetch`.
Then `git diff ...origin`.

If you see that there have been changes made,
you need to pull those changes into your local repo. This is done by the command
  `git pull origin branch`. Origin is the remote repo.
  Branch is the name of the branch you are pulling from. You can pull from
  any branch in the repo. Often you will be pulling changes from a branch other than master. Once you have pulled in any
  changes, you will then have a complete copy of everything that has been done in the repo since the last time you pulled.
  You should be, at this point, ready to begin working on your files

## Sending Your Work to the Repository

When you have completed working on your files you can send your changes to the remote repository.
Let's go over the basic procedure for this now.

* Open a terminal.

* Navigate to your working directory.

* Type `git status`. This will show you what files have been changed.
  The changed files are rendered in red.

* Type `git add` with the name of the file you wan tto add to the staging area.

* Type `git status` again. You should see the files you added now rendered in green. These
  are now in the staging area.

* Type `git commit -m [A short description of what was done]`

* Git will send the changes to the remote. And your done.

One of the actions that cannot be done from the command line is the `pull request`. The `pull request` cannot be done from
the command line. It must be executed at the GitHub website.

* Go to your account in GitHub.

* Select the repo you wich to make to pull request to.

* Create your pull request.

That is all there is to it.