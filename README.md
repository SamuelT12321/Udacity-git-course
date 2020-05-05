## Udacity-git-course (HTML)

This project is done by following **Udacity git online course**

### `This Project show case how to use below Git commands`

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
    
    
#### Add Commit to Repo  ####  

<a herf="https://git-scm.com/book/en/v2/Getting-Started-First-Time-Git-Setup">1.6 Getting Started - First-Time Git Setup</a>

    # To add change or file to stage. {} = either one 
    * git add {FileName}{.}
    
    # To add change to repo
    * git commit
    
    # To see change have not yet committed 
    * git diff
 
Git Ignore file
  git ignore any file that start with a dot and will read .gitignore file to ignore add 
  <a herf="https://en.wikipedia.org/wiki/Glob_(programming)"> globbing </a>
    
#### Addictional Required Commands in git bash ####
    *  ls - used to list files and directories
    *  mkdir - used to create a new directory
    *  cd - used to change directories
    *  rm - used to remove files and directories
    *  q  -used to exit the bash state

<a herf="https://git-scm.com/docs/git-diff"> Git Docs page </a>

### License
myreads is Copyright ©2020 Samuel tam. terms specified in the <a href="https://github.com/SamuelT12321/myreads/blob/master/LICENSE.txt">LICENSE</a> file.
