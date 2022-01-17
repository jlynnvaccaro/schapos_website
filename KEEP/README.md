# How to set up and edit the website
J Vaccaro

Prereqs:
* Ruby
* Git

## Repository content (code, files, etc.)

There are several ways to edit and add content. This section covers the git terminal instructions for setting up and editing your repository content locally.

### Clone the repository locally

You can either use the terminal or the Github GUI. I'll give directions for the terminal, but you'll be looking to click the corresponding buttons in the GUI.

* Open the terminal
* Navigate to the folder where you want the repo using the ``cd'' command.
* Clone the repo with ``git clone https://github.com/jlynnvaccaro/schapos_website.git''
* Now, all of the files are on your computer locally, so you can edit them in a text editor of your choice. Use the edit instructions to publish your changes.

### Edit the repository locally

The process is *pull*, *edit*, *status*, *add*, *commit*, *push*. Make sure to debug this process with a minor change before making substantial changes.

First, download the latest changes from your repository. 
* Open a terminal, and navigate into the repo folder using ``cd''.
* Use the command ``git pull'' to pull the latest changes from Github.

Then, make your edits to any files in a text editor of your choice.

To check which files have been changed, use the command ``git status''. This will not make any changes to the repository, but instead will display what files have been modified, added, or removed.

If you would like to add a file, or accept all changes to a file, use ``git add FILENAME''. You can also use ``git add *'' or ``git add *.txt'' in order to add all files or all txt files, respectively. To remove a file from the git repository, use ``git rm FILENAME''. If you have a file in the local repository that you do not want git to track, you can use ``git ignore''.

Once you are done with changes, or have made substantial changes that you would like a snapshot of, you should *commit* the current progress. Use the command ``git commit -m "Message describing the changes"''.
* For example, if I had just finished fixing a broken link, I might use the message ``fixed broken link on the CV page''.

Locally, your git repository will keep track of your commits, and you can revert back to previous commits. You don't need internet access while making these changes locally. 

To send these commits to the Github repository, use ``git push''. By default, this will send your changes up to the Github repository, and you should then see the changes reflected in your website. On shared projects, I use ``git pull'' again before pushing, but since you will be the only person making changes to your repo, this is not strictly necessary.

If you have issues with merges, that means that you have multiple versions of the same folder in different places, and git does not know which changes to keep and discard. Check out git documentation if this happens. Try not to keep multiple local versions of your files/repo in order to avoid this issue.

### Edit the repository on Github

You can edit text files and upload/delete content directly on github. After each change, you will be prompted to commit the change. If you are editing your repo in multiple ways, e.g. locally and on Github, then make sure to pull your latest changes before continuing to edit.

### Edit content that you would not like to publish yet

If you want you renovate the website significantly, then you may want to setup a separate branch in order to work on the extensive changes. Then, once you are happy with the newer version, you can set the Pages site to use the newer branch. Adding branches can make it more difficult to keep track of the status of your repo, and look up git branch documentation for more info.

## Github pages settings (url address)

In addition to editing the content, you can edit the Github Pages settings on Github. 

* Open Github, and navigate to the repository.
* Click Settings >> Pages.
* Make any changes that you would like.
* * Source: change which folder the code from the website comes from. Since this repository is only website code, you should not change this.
* * Theme chooser: You can add stylesheets to the website in order to change the theme.
* * Custom domain: You can serve your site from a domain other than the Github default.