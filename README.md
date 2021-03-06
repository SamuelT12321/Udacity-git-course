## Udacity-git-course (HTML)

This project is done by following **Udacity git online course**

This Project show case how to use below Git commands

<a href="https://www.atlassian.com/git/tutorials/syncing">git remote, pull, fetch , push </a>

#### First Time Git Configuration: ####

    # sets up Git with your name
    *  git config --global user.name "<Your-Full-Name>"

    # sets up Git with your email
    *  git config --global user.email "<your-email-address>"

    # makes sure that Git output is colored
    *  git config --global color.ui auto

    # displays the original state in a conflict
    *  git config --global merge.conflictstyle diff3

    *  git config --list

    #Sublime Text Setup
    *  git config --global core.editor "'/Applications/Sublime Text 3.app/Contents/SharedSupport/bin/subl' -n -w"

#### For Creating a project and check status and log  ####

Make sure your are on the project directory 

    # sets up all of the necessary files and directories that Git will use to keep track of everything. 
    *  git init
    
    # clone github repo 
    *  git clone https://{your repo URL}
    
    # To check the state of our repo
    *  git status
    
    # To check log of commit
    *  git log  *  git log --oneline
        to scroll Down [J] /scroll Up [K]
        *  Press q key to return regular cmd
    
    # To display the files that have been changed in the commit
    *  git log --stat
    
    # To display the actual changes made to a file. {} = optional
    *  git log -p {SHA fdf1223}
    
    # To display one commit changes. {} = optional
    *  git show {fdf8853}
    
    # To show some details that are hidden in the default view 
    * git log --decorate
    
    # Try me out 
    * git log --oneline --decorate
    
#### Add Commit to Repo  ####  

<a href="https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup">1.6 Getting Started - First-Time Git Setup</a>

    # To add change or file to stage. {} = either one 
    * git add {FileName}{.}
    
    # To add change to repo
    * git commit
    
    # To see change have not yet committed 
    * git diff
 
`Git Ignore file
  git ignore any file that start with a dot and will read .gitignore file to ignore add` 
  
  <a href="https://en.wikipedia.org/wiki/Glob_(programming)">globbing</a>
  
#### Add Tagging ####

    # Add tag to current tag 
    * git tag -a v1.0
    
    # To Verify Tag 
    * git tag 
    
    # To make a tag in the previous commit with SHA
    * git tag -a beta a65e14
    
    # To delete a Tag
    * git tag -d v1.0
    
<a href="https://git-scm.com/docs/git-tag"> Git Tag Docs </a></br>
<a href="https://git-scm.com/book/en/v2/Git-Basics-Tagging"> Git Basics- Tagging from the git book </a>

#### Branching ####

    # To list all branch
    * git branch
    
    # To Create a Branch (make sure your are on current branch ..like master)
    * git branch sidebar
    
    # To switched branch (make sure you have all your work added and commit before checkout)
    * git checkout sidebar
    
    # To create a branch with SHA 424266e
    * git branch alt-sidebar-loc 424266e
    
    # To Delete a branch
    * git branch -d sidebar
    
    # To create a branch call samuel-branch-for-awsome-changes and switch over immediately
    * git checkout -b samuel-branch-for-awsome-changes
    
    # To create a branch call footer from copying master branch and switch over immediately
    * git checkout -b footer master
    
    # To see all branch at once 
    * git log --oneline --decorate --graph --all

#### Merging ####
    
    # To merge branch "footer" to your current brach master (make sure to git checkout to master)
    * git merge footer
    
##### Merge Conflict Indicators Explanation #####
The editor has the following merge conflict indicators:

    *  <<<<<<< HEAD everything below this line (until the next indicator) shows you what's on the current branch
    *  ||||||| merged common ancestors everything below this line (until the next indicator) shows you what the original lines were
    *  ======= is the end of the original lines, everything that follows (until the next indicator) is what's on the branch that's being merged in
    *  >>>>>>> heading-update is the ending indicator of what's on the branch that's being merged in (in this case, the heading-update branch)

    
<a href="https://git-scm.com/book/en/v2/Git-Branching-Basic-Branching-and-Merging#Basic-Merging"> Basic Merging from Git Book </a></br>
<a href="https://git-scm.com/docs/git-merge"> git-merge from Git Docs </a></br>
<a href="https://www.atlassian.com/git/tutorials/using-branches/git-merge"> git merge from Atlassian blog </a>

##### Undoing changes #####

    # To forgotten files to commit
    * git commit --amend
    
    # To revert a specific commit
    * git revert <SHA-of-commit-to-revert>

    # Resetting is Dangerous make sure you know what you are doing :)
    * git reset <flags> <reference-to-commit>
        # Flags 
        * --mixed    <-this will delete the repository master head and move repo master head to working directory
        * --soft     <-this will delete the repository master head and move repo master head to Staging index
        * --hard     <-Trash it and never find it again 
    
    # Backup Branch, before resetting is good to back it up 
    * git branch backup
    
    # To merge back up
    * git checkout -- index.html   <- reverst all the changes before merge backup
    * git merge backup

<a href="https://git-scm.com/docs/git-revert">git-revert from Git Docs</></br>
<a href="https://www.atlassian.com/git/tutorials/undoing-changes">git revert Atlassian tutorial</></br>
<a href="https://git-scm.com/docs/git-reset">git-reset from Git docs</></br>
<a href="https://git-scm.com/book/en/v2/Git-Tools-Reset-Demystified">Reset Demystified from Git Blog</></br>
<a href="https://git-scm.com/book/en/v2/Git-Tools-Revision-Selection#Ancestry-References">Ancestry References from Git Book</></br>
<a href="https://github.com/jlord/git-it-electron">try tackling some Git challenges with the Git-it app</a></br>
    
#### Addictional Required Commands in git bash ####
    *  ls - used to list files and directories
    *  mkdir - used to create a new directory
    *  cd - used to change directories
    *  rm - used to remove files and directories
    *  q  -used to exit the bash state

<a href="https://git-scm.com/docs/git-diff"> Git Docs page </a>

### License
myreads is Copyright ©2020 Samuel tam. terms specified in the <a href="https://github.com/SamuelT12321/myreads/blob/master/LICENSE.txt">LICENSE</a> file.
