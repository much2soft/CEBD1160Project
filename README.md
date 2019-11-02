# CEBD1160Project
Group Project for CEBD1160

Group Members:

Abdullah

Bhargav

Claire

Christian

Michael

## How To Download and Upload files to Git

To clone this workspace use https or ssh.  https is easier but you will be asked for your
Git password each time you interact with Git so it's ok at first but can get tiresome.

Using https:

  git clone https://github.com/much2soft/CEBD1160Project.git

Using ssh:

  git clone git@github.com:much2soft/CEBD1160Project.git

This will create a folder with all the files on your local PC called "CEBD1160Project".  After it's cloned, go to the folder

  cd CEBD1160Project

This folder is being tracked by Git, so all changes made here can be uploaded to
the public folder.  Once you make a change to a file in this folder, you can see which files
have changed and which branch you're on by doing

  git status

### Method 1: Merge directly to master

Once you make a change, for example to README.md, you need to stage your change by doing

  git add README.md

or to add changes from all files modified,

  git add .

The following command will bring up a screen where you can type in your commit message.
The screen that comes up varies depending on your OS.

  git commit

Finally, push your change to the Public server master branch by doing

  git push origin master

Your change will now be public!

If somebody changed the file you were also changing, the above command may fail.
You can attempt to merge their changes into yours by doing "git pull", but the merged file
might not open correctly in Jupyter Notebook!
BACKUP YOUR WORK INTO A DIFFERENT FOLDER FIRST!
The easiest thing to do is to then REVERT your own changes (UNDO ALL) using

  git checkout .

Then now you can pull the most recent version from the server:

  git pull origin master

Now manually re-do your changes in Jupyter Notebook, then go back to the "git add ." step above.

Note that if everybody works on a different file, Git will automatically merge in changes and you
won't need to worry too much about merge conflicts.  So this will probably be the easiest approach.

Also, for now there is only a master branch, which is also the simplest to understand right now.

### Method 2: Open a Pull Request

Make sure your master branch is up to date.  To do this, first make sure you're on the master branch

  git checkout origin/master
  
Now get the laster version from the server:

  git pull origin master
  
Once master is up-to-date, create a submit branch for you to work on, for example, "test_branch":

  git checkout -b test_branch

Now you can make changes to your files in your branch, such as adding a file or modifying one.
Once you have a change and you are ready to open a Pull Request, first add your changes.  Let's
say you changed a file named "test_file.txt", add that one:

  git add test_file.txt

Now create a commit the changes to your local branch with a commit message:

  git commit

Finally, push the changes from your branch to the server.  In this case we are pushing our
local version (origin) to a new branch on the server with the same name called "test_branch":

  git push origin test_branch

Now, go to the Git Web interface and you will see a Banner that says "Open Pull Request".
Click that, then add people as reviewers by clicking on the Gear icon on the top right.
Once the reviewers approve, click on "merge" and then your branch will be merged to the
master branch.

Your changes are now public!

At this point you can safely delete your "test_branch" on the server using the Git Web interface,
since the purpose of this branch was just for submission.  There is button to do that after you
merge your change.

You can also delete your submit branch on your local workspace. To do this, first go back to
the master branch:

  git checkout origin/master

Now delete your submit branch

  git branch -D test_branch


