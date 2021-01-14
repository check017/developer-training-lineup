# GitHub

GitHub is a website that allows developers to share code files. It allows you to pull in the repos of other developers,
make changes, and send the files back. It also allows you to do the same.GitHub uses Git version control software to
achieve this. However, GitHub is not Git.
It just uses Git to make it easy for developers to share their code.
It is recommended that you become comfortable using Git before you dive into GitHub.
In order to discuss GitHub intelligently,
it is first necessary to define a few words that are
used on the platform.

## Terms

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
The branching feature is used for more than just experimenting.
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
    - This is the action of retrieving data from remote repository. Any changes present in the remote will be merged
    with your local repo.

* `fetch`
    - This command will check for any changes made to the remote (main) repository, but it does not tranfer any files or
    make any changes.

* `diff`
    - This command will show the changes made before and after you have made changes.
  It will also show any changes that have
  been made in the remote compared to your local repo

* `pull request` move this
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

* Once you have saved your files, you need to send them to `remote`.
  To do this you give the command `git push [name of remote] [name of branch]`

One of the actions that cannot be done from the command line is the `pull request`. The `pull request` cannot be done from
the command line. It must be executed at the GitHub website.

* Go to your account in GitHub.

* Select the repo you wich to make to pull request to.

* Create your pull request.

That is all there is to it.

We need to check to see if there have been any changes made since the last time you pulled from the repo. Type `git fetch`.
Then `git diff ...origin`.
