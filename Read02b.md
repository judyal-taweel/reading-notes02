# Version Control
#### is a system that allows you to revisit various versions of a file or set of files by recording changes,
#### by utilizing a Version Control System (VCS), mistakes with files can easily be rectified.
The need for collaboration within a developer team on a single file or set of files led to the advent of the Centralized Version Control System (CVCS),
 If a CVS goes down, collaborators cannot work with each other on a file or save changes and new versions To prevent this type of catastrophic loss,
 a DVCS allows clients to create mirrored repositories to replace any lost information.

# Git
Git is a DVCS that stores data in a file system made up of snapshots. Each time you save a changed version of your project — called commit — Git creates 
a snapshot of the file and stores a reference to it. If the file has not changed, Git only stores a reference to the already-stored identical version of it.
Git mostly relies on local operations because most necessary information can be found in local resources.
Every single change applied to any file or directory is tracked by Git. And, as the gatekeeper, Git will always detect file corruption or loss of information in transit.

#### Files in Git can reside in three main states:
1. Committed : Data is securely stored in a local database
1. Modified : File has been changed but not committed to the database
1. Staged : Flagged a file’s changed version to be committed in the next snapshot

### Download Git
#### Git can be installed in three ways:
- Install as a package
- Install via another installer
- Download and compile the source code.

### method for installing Git if:

#### 1. Mac OS X
- running Git from the Terminal. If Git is not installed, you will see a prompt for installation.
- You can also download Git by visiting this link "http://git-scm.com/download/mac".
- Download GitHub for Mac via ththis link "http://mac.github.com".

#### 2. Windows
- You can download Git by visiting this link "http://git-scm.com/download/win".
- Install Git as part of the GitHub for Windows install "http://windows.github.com".

#### 3. Linux
- For Fedora: `$ sudo yum install git`
- For Ubuntu: `$ sudo apt-get install git`
- To download Git for Linux, visit this link "http://git-scm.com/download/linux"

### Graphical Clients
You can access a variety of GUI clients for Mac, Windows, and Linux via this link:
"https://git-scm.com/downloads/guis"

### Initial Customization
- Configuration of Variables : Git tool called git config allows the setting of configuration variables that control aspects of Git’s operation and look.
- Identity Setting : 

Type the following into Terminal or Command Line:

`git config --global user.name "Jane Smith"
git config --global user.email "example@email.com"`

And to confirm that you have the correct settings:

`git config --global user.name (should return Jane Smith)
git config --global user.email (should return example@email.com)`

### Default Text Editor

`$ git config --global core.editor emacs`

### Check Settings
To check settings, use the `git config --list` command.

### Getting Help
There are three ways to get more information on a particular command:
1. `git help command`
1. `git command --help`
1. `man git-command`

# Setting up a Git Repository
#### Steps to import an existing project or directory into Git using the Terminal or Command Line:
1. Switch to the target project’s directory: `$ cd test (cd = change directory)`
1. Use the git init command: `$ git init`
1.  perform an initial commit to start tracking these repository files:
- `$ git add *.c`
- `$ git add LICENSE`
- `$ git commit -m “any message here”`

### Cloning
`$ git clone https://github.com/test`

# Workflow
### Local Repository Structure
###### The local Git repository has three components:
1. Working Directory: The actual files reside here.
1. Index: The area used for staging
1. Head: Points to the most recent commit

###### Saving Changes
- Tracked
- Untracked

#### The Life Cycle of File Status
After you edit a file, Git flags it as modified because of changes made after the previous commit,You stage the modified file
Then, you commit staged changes.

#### Check File Status
To determine the state of files `$ git status`

#### Tracking and Staging a New File
- Single File using the following format: `git add filename`
- All Files using the following command: `$ git add *`

#### Committing a File
you commit the changes and record: `$ git commit -m “made change x,y,z”`

#### Committing All Changes
`$ git commit -a`

#### Pushing Changes
`$ git push origin master`

####


































