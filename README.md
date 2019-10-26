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

Once you make a change, you need to stage your change by doing

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
You can attempt to merge their changes into yours by doing this, but the merged file
might not open correctly in Jupyter Notebook!
BACKUP YOUR WORK INTO A DIFFERENT FOLDER FIRST!

  git pull origin master

Note that if you are working on a different file, Git will automatically merge in changes and you
won't need to worry too much about merge conflicts.  So this will probably be the easiest approach.
For now there is only a master branch.

