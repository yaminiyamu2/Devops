#Git:-
       Git is a popular version control system.It was created by "Linex torvalds in 2025",and has been maintained by Junio Hamano since then.
	It is used for:
->Tracking code changes.
->Tracking who made changes.
-> coding collaboration.
 1.Mange projects with Repositories.
 2.Clone a poject to work on a local copy.
 3.control and Track changes with staging and commiting.
 4.Branch and merge to allow for work on different parts and versions of a projects.
 5.Pull the latest version of the projects to a local copy.
 6.Push local updates to the main projects.

#version control system Features:-
       version control system is a s/w which is a source code repository with freatures such as:
 1.Multi-user support.
 2.History.
 3.support for multiple releases/customers in a way to work in parallel in same repository.
 4.user mangement.
 
 #Git Basic workflow in local system:-
        In git we have 3 areas in repository
 1.Working Tree: Here we make changes.
 2.Staging Area: Here we move/categorize changes.
 3.Local Area:   Hare we see the changes for one freature/defect as a commit. 
 
 #Git workflow:-
        The Git workflow defines a static branching model designed around the project release. This workflow doesn't add any new concepts beyond 
	what's required for the feature branch workflow.
 1.Modified
 2.Staged
 3.committed
	 
	step by step workflow
-> Developer:
 1.For Developing Features.
 2.For fixing issues.
->Tester:
   Automation Testers devlop test scripts for automation.
->DevOps:
 1.For maintaining Devops pipelines.
 2.For storing
    a) K8s mainfects(Kubernet)
	b) Docker files
	c) Terraform templates/modules
	d) Ansible Playbook
	
Ways OF WORKING
 1.GUI: Graphical user interface
      A Graphical user interface is a form of user interface that allows users to interact with electronic devices through Graphical icons and audio indicaters such as primary notation.
 2.Commandline:
      CLI is a command line program thst accepts text input to execute operating system functions.
	a) Command line interface
	b) Command line interpreter
	c) command line input
	
#Git configurations(Git config):
     The Git config command is a convenience function, that is used to set Git configuration value on a global/Local project level. 
  These configuration levels correspond to .gitconfig text files. Executing gi config will modify a confiuration text file.
  Git Has configuration of 3 Types:
1.System config.
2.Global config
3.Local config.
To deal with config we hace command
**git config --help**
command prompt:-
git config --global user.name (username)
git config --global user.email (email I'd)	

#Git init:
   Initalize the folder wirh git init to make it a git repository.
**git init** 

#Git commits:
    Since we have finished our work, we are ready move from Stage to commit for our repository. 
Adding commit keep tracl of our programs and changes as we work.
Git considers each commit changes point or "Save point"
Record changes to the repo.
**git commit**
command prompt:-
PS C:\temp\learningGit\ltsalesman> git commit --help
By adding clear meaasge to each commit it is easy for yourself to see what has changed and when
The commit command performs a commit & the -m "message" add a meaasege
The Staging Env has been commited to our repo
command prompt:-
PS C:\temp\learningGit\ltsalesman> git commit -m "required message"

#Git Log:
To view the history of commit for a repository, you can use the Log command
**git log**
->Git log short form is called oneline
**Git log --oneline**
command prompt:-
PS C:\temp\learningGit\ltsalesman> git log

#Git ignore:
We can configure git to ignore some files or folders . To do this we need to create a file called as .gitignore in the root folder of the repository.
**.gitignore**
command prompt:-
PS C:\temp\learningGit\ltsalesman> git status
PS C:\temp\learningGit\ltsalesman> git add - A
PS C:\temp\learningGit\ltsalesman> git status
PS C:\temp\learningGit\ltsalesman> git commit -m "add meassage(ex:added ignore files)"

#Git Restore:
     Restore specifed paths in the working tree with some contents from a restore sourse. If a path is tracked but does not exist in the restore,
   it will be removed to match the sourse.
   The command can also be used to restore the content in the index with --staged
**git restore --staged** 
command prompt:-
PS C:\temp\learningGit\ltsalesman> git restore --staged src\app.py
PS C:\temp\learningGit\ltsalesman> git status
 by Default,if --staged is given , the contents are restored from HEAD , otherwise from the index git-restore Documentation.
command prompt:-
PS C:\temp\learningGit\ltsalesman> git commit -m " added start and stop app"
PS C:\temp\learningGit\ltsalesman> git log --oneline

# git clean -fd:
   To remove all the untraked files from a specific folder.
**git clean -fd <path>**

#git reset:
---> Soft:
        Does not touch the index file or the working tree at all (but resets the head to <commit>, just like all modes do). 
      This leaves all your changed files "changes to be commited", as Git status would put it.
**git reset --soft**
            command prompt:- (Git Bash)
            yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (master)
            $ git reset --soft
---> Hard:
        Resets the index and working tree.Any changes to tracked files in the working tree since <commit> are discarded.
      Any untracked files or directories in the way of working any tracked files are simply deleted.
**git reset --hard**
             command prompt:- (Git Bash)
             yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (master)
             $ git reset --hard
---> Mixed
        Resets the index but not the working tree(i.e., the changed files are preserved but not marked for commit) and reports what has not been 
      updated.This is the default action.
**git reset --mixed**
             command prompt:- (Git Bash)
             yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (master)
             $ git reset --mixed   

#Git checkout:
    Switch branches or restore working tree files
**git checkout <commit>**
command prompt:- (1)
PS C:\temp\learningGit\ltsalesman> git log --oneline
PS C:\temp\learningGit\ltsalesman> git ckeckout <commit i'd>
PS C:\temp\learningGit\ltsalesman> git log --oneline
command prompt:- (2)
PS C:\temp\learningGit\ltsalesman> tree /F

#Git branches:
   Git branches are effectively a pointer to a snapshot of your changes.When you want to add a new feature or fix a bug no matter how big or 
how small you spawn a new branch a new branch to encapsulate your changes. This makes it harder for unstable code to get merged into 
the main code base, and it gives you the chance to clear up your future's history before merging it into the main branch.
**git branch** 
command prompt:- 
PS C:\temp\learningGit\ltsalesman> git branch

#Git merge:
   Merge is an operation to bring all the changes from the one branch to another. 
->Conflict arises when git tries to merge the changes and findouts conflicting information form two diffrent references. 
**git checkout master**
**git mearge (example: marutisuzuki)**
command prompt:- (Git Bash)
yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (master)
$ git checkout master
yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (master)
$ git merge marutisuzuki
yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (master)
$ git log --oneline

#git rebase:
 Rebasing is the process of moving or combining a sequence of commits to anew base commit 
**git rebase main**
command prompt:- (Git Bash)
yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (feature_1003)
$ git rebase main

#Git cherry-pick:
   Rebasing is the process of moving or combining a sequence of commits to anew base commit. 
**git rebase main**
command prompt:- (Git Bash)
yamuy@yamini MINGW64 \c\temp\learningGit\ltsalesman (feature_1003)
$ git rebase main

#Git reflog:
   This command manges the information recorded in the reflogs.
-->reference logs/reflogs,record when the tips of branches and other references were updated in the local repository.
   Reflogs are useful in various git coomand,to specify the old value of a reference.
**git reflog**

 #Git clone:
      Clone is use when you have a remote repository but you don't have local version of it.
**git clone**

#Git Pull:
    Pull is there is remote repo and you have a local repo and now you want to get a latest changes.
**git pull**

#Git pull vs Pull-rebase:
     Pull is generally done a local changes if you only get a latestversion.
	 Pull-rebase doesn't create merge commit.
    
	 


	
	 
 