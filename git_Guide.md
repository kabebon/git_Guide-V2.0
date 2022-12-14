# Hello, world!
## Git instruction is here :0, let's check your gained experience.

1. Starting from installing the git from the [official website]. 
2. When finished, install [Microsoft Visual Studio Code]. 
3. Create a folder with any name on your desktop. For example: "gitBeginner"
4. Open MVSC and open your empty folder using: File > Open folder and choose your folder.
5. In opened folder create a file with extension __.md__ with any name.
That's it! You are ready to communicate with git, but wait. Let's open a terminal and verify your git installation with a command <span style="color:orange"> __git --version__ </span>. If you see a version of git, congratulations! You are in the game :)

## Some commands

*  __git init__ - Initializes the folder in which git will start tracking the changes. A hidden folder is created in the folder.git 

* __git status__ - Shows the current state of the git, whether there are changes that need to be committed (saved).

* __git add__ - adds the contents of the working directory to the index (staging area) for a subsequent commit. This command is given after adding files. It is not necessary to write the whole name: the terminal will fill in the data automatically.

* __git commit__ - The git commit command takes all the data added to the index using git add and stores their cast in the internal database, and then shifts the pointer of the current branch to this cast.

* __git log__ - Change log. Before switching the file version to Git, use the git log command to see the number of saves.

* __git checkout__ - Switching between versions. To work, you need to specify not only the commit you are interested in, but also return to the one where we work using the command git checkout master.

* __git diff__ - Shows the difference between the current file and the saved one
Before switching the file version to Git, use the git log command to see the number of saves. 

Have a nice day, <font size ="4"> __Ivan :)__ 😃

[official website]: <https://git-scm.com/book/en/v2/Getting-Started-Installing-Git>
[Microsoft Visual Studio Code]: <https://code.visualstudio.com/>
***
## Now we have the second stage of our jorney: creating branches, merging and resolving conflicts :)

### *Creating branches*

You can create a branch using the git branch command.
This should be done in the repository folder: __git branch "name of the new branch"__
If we have several versions of the draft, we can display the branch where we are
with the __git branch__ command. Remember that the first branch of the local repository is called <font size ="5"> __Master__ </font>. If you need to switch from one branch to another, call the __git checkout "branch name"__ command.
***
### *Merging*
When we edit the text/code in the current branch, there is no automatic merging: you can create one document in different versions in different branches. The __git log__ command will show the status of newer versions of the project. But if we call this command from the "freshest" branch, we will not see the source file.

Let's say we are completely satisfied with the drafts and we need to make changes so that the information appears in the clean. There is a __git merge__ command for this.
To merge any branch with the current one, call __git merge "name of the branch"__ to merge with the current one"
***
### *Deleting branches*

If the branch is no longer needed, you can delete it using __git branch -d "name of the branch"__
***
### *Adding an image*

It is not customary to add image files in Git, they are stored on third-party media. To exclude unnecessary files from downloading, there is a git ignore command.
***
### *Conflicts*

When working in two branches at the same time, a situation may arise when we changed a block of text in one and the other branch in different ways. If we then try to merge these branches, Git will report a conflict and offer to choose which changes to write. Therefore, the project must have one responsible user in the  repository, who has the right to merge and resolve conflicts.
***
### *Visualization of all branches*

__git log --graph__
The -graf key in conjunction with the log command allows you to display commits as a tree.
***

## Now we have the third part of our journey: connect to remote repository :)

### *Downloading from the current repository and merging with your own version*

Master working with remote repositories that are located not on a local, but on a remote machine, for example, on a server. You can copy the external repository to your PC with the __git clone__ command. The git clone composite command: it not only downloads all the changes, but also tries to merge all the branches on the local computer and in the remote repository.
***
### *git pull*

This command allows you to download everything from the current repository and automatically merge with our version.
***
### *git push*

The git push command will help you send your version of the repository to an
external repository. The first time you use it, you need authorization.
***
### *How to set up collaboration*

1. Create an account on GitHub.com
2. Create a local repository
3. “Make friends” with your local and remote repositories.
GitHub will tell you how to do this when creating a new repository
4. Send (push) your local repository to the remote one (on GitHub), at the same time, you may need to log in to the remote repository
5. Make changes “from another computer”
6. Pull the current state from the remote repository
***
### *pull request*

The command to propose changes. in large companies, one responsible for the project creates an account. Other users give the pull request command. You need to propose changes on GitHub in a separate branch. First, the user copies the repository to his computer, makes a fork of the repository, then clones the version on his PC, creates a branch with the proposed changes, sends the changes with a push command to his GitHub account and gives the pull request command.
***
### *How to make a pull request*

Making (a branch) of the fork repository Making the git clone version of the repository OUR OWN Create a new branch and make our own changes to IT Fixing changes (making commits) We are sending our version to our GitHub On the GitHub website, click the pull request button.