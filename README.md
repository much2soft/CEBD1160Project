# CEBD1160Project

This is a group project for course CEBD1160 at Concordia University in Montreal.  The project work is a simplified version of the Kaggle competition where we are focusing on using different techniques to predict trends in the item sale data over time.  All work is done in Python 3 in Jupyter Notebook using the Anaconda environment. The data must be downloaded from the Kaggle competition and placed into the "data" folder before running the examples:

https://www.kaggle.com/c/competitive-data-science-predict-future-sales/overview


# Libraries used

Pandas

Matplotlib

Prophet

Keras / Tensorflow

## Group Members:

Abdullah (abdullahcn)

Bhargav (bparekh2)

Christian (tchatec)

Claire (C-SUN19)

Michael (much2soft)

### Opening a Pull Request

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
local version (origin) to a new branch on the server with the same name called "test_branch".
Once you push your branch to the server, your changes are public and other group members can see
your work:

  git push origin test_branch

Now, go to the Git Web interface and you will see a Banner that says "Open Pull Request".
Click that, then add people as reviewers by clicking on the Gear icon on the top right.
Once the reviewers approve, click on "merge" and then your branch will be merged to the
master branch.

Your changes are now public and in the master branch!

At this point you can safely delete your "test_branch" on the server using the Git Web interface,
since the purpose of this branch was just for submission.  There is button to do that after you
merge your change.
