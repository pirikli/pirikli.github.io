---
title: Introduction to Git Version Control
date: 2025-02-14 21:42:00 +0330
categories:
  - Version Control
  - Git
  - GitHub
tags:
  - git
  - github
  - versio_control
layout: post
---
# <a id="top"><font color="red">📮Introduction to</font></a>  
![Version Control](https://git-scm.com/images/logos/2color-lightbg@2x.png)  
**By <font color="royalblue">[Pirikli](https://github.com/pirikli)</font>**

**<font color="red">Table of contents</font>**  
| [📌Concepts](#head1) | [📌Shell commands](#head2) | [📌Git from scratch](#head3) | [📌Git workflow](#head4) | [📌Comparing file](#head5) | [📌commit Structure](#head6) | [📌Undoing Changes before Commit](#head7) | [📌Restoring & Reversing](#head8) | [Configuring Git](#head9) | [Handling Conflicts](#head10) | 

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

## <font color="purple"><a id="head1">📚Concepts📚</a></font>

### <font color="#00FFFF">🌀version:</font>  
- **🎯<font color="green"><mark>Contents of a file and its Metadata</mark>(author, location, type, time...) at a given point in time.</font>**  

### <font color="#00FFFF">🌀version Control🛂</font>  
- **🎯<font color="green"><mark>systems and processes</mark> which manage `changes` made to files and directories in a project. they allow us to keep track of what we did when, to undo any changes we don't want, and collaberate with others in a project. </font>**

### <font color="#00FFFF">🌀[Git](https://git-scm.com)</font>
- **🎯<font color="green">a popular <mark>version control system</mark> for computer programming and data projects. Tracking code changes
Tracking who made changes
Coding collaboration</font>**

### <font color="#00FFFF">🌀Github</font>  
- **🎯<font color="green"> a cloud-based <mark>git repository hosting</mark> platform.</font>**    
                                                              
### <font color="#00FFFF">🌀Repository</font>
* contains 2 parts:
> **<font color="green"> ➊ our files and directories.</font>**    
>   
> **<font color="green"> ➋ .git (a directory located in the main directory of repo) in which Git records extra  information about project’s history.</font>**    
>
>> 💾 **<font color="purple"> If your repo is:</font>  <font   color="#F39C12">/home/user/myrepo</font>**  
>>   
>> 💾 **<font color="purple"> your repo's history is saved to:</font>  <font color="#F39C12"> /home/user/.git</font>**

Local repo or repository: A local directory containing code and files for the project    
Remote repository: An online version of the local repository hosted on services like GitHub, GitLab, and BitBucket    
Cloning: The act of making a clone or copy of a repository in a new directory    
Commit: A snapshot of the project you can come back to    
Branch: A copy of the project used for working in an isolated environment without affecting the main project   
Git merge: The process of combining two branches together 

More advanced definitions   
.gitignore file: A file that lists other files you want git not to track (e.g. large data folders, private info, and any local files that shouldn’t be seen by the public.)    
Staging area: a cache that holds changes you want to commit next.   
Git stash: another type of cache that holds unwanted changes you may want to come back later   
Commit ID or hash: a unique identifier for each commit, used for switching to different save points.   
HEAD (always capitalized letters): a reference name for the latest commit, to save you having to type Commit IDs. HEAD~n syntax is used to refer to older commits (e.g. HEAD~2 refers to the second-to-last commit).   


 # <font color="purple"><a id="head2">🐚some shell commands🐚</a></font>


```bash
%%bash
#🪄magic command for executing Bash codes on jupyter🪄

pwd  #🎯stands for 'print working directory'
ls     #🎯stands for 'list storage'
ls -a  #🎯to see hidden files like .git
```

#### <font color="#00FFFF">🌀commands for creating and modifying text files🌀</font>


```python
nano text_file.txt #🎯to save and exit(ctrl+o,Enter, ctrl+x)
echo "This is a new text file" > text_file.txt`

#👆single `>` will overwrite everything

echo "This is the second line" >> text_file.txt`

#👆double `>>` will append contents to file.

git --version  #🎯check for git version
# Note: running this cell here will throw errors,
#because these are shell commands and need terminal to execute.
```

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# 📝<font color="purple"><a id="head3">Git from Scratch, on [Ubuntu](https://ubuntu.com/):</a></font>📝 

### <font color="#00FFFF">🚪➊-Enter Terminal:</font>  `ctrl+Alt+T`

### <font color="#00FFFF">💱➋-update and upgreade:</font>  


```python
💲sudo apt-get update  
💲sudo apt-get upgrade  
```

### <font color="#00FFFF">📥➌- Install git:</font> 


```python
💲sudo apt-get install git 
```

4- check if installation was successful?
`git --version`

### <font color="#00FFFF">📁➍- Create a local repository, if you're woriking locally:</font> 


```python
💲mkdir /home/user/MyFirstRepo
```

### <font color="#00FFFF">🏃➎- Go to your repo:</font> 


```python
💲cd /home/user/MyFirstRepo
```

### <font color="#00FFFF">🔑➏- initial git:</font>  


```python
💲git init
```

### <font color="#00FFFF">🔗➐- Configure connection:</font>    
Important tags to determine the scope of configurations  
Git lets you use tags to determine the scope of the information you’re using during setup  

Local directory, single project (this is the default tag)   
$ git config --local user.email “my_email@example.com” Also if you don't specify any key; the user name and email will be set for just the current repo!  

All git projects under the current user   
$ git config --global user.email “my_email@example.com”    

For all users on the current machine   
$ git config --system user.email “my_email@example.com” 

Other useful configuration commands   
List all key-value configurations  
$ git config --list  

Get the value of a single key  
$ git config --get <key>  

Setting aliases for common commands  
If you find yourself using a command frequently, git lets you set an alias for that command to surface it more quickly  

Create an alias named gc for the “git commit” command   
$ git config --global alias.gc commit   

$ gc -m “New commit”   

Create an alias named ga for the “git add” command   
$ git config --global alias.ga add   


```python
💲git config --global user.name "my username"  #wrap it in a quoutations if your user name has space.
💲git config --global user.email  my.email@domain.com
```

### <font color="#00FFFF">💼➑- Create new *repository* on github and connect to it:</font> 


```python
💲git remote origin https://github.com/username/MyRepo.git    
#if you're stuck and recieve errors, try👇:    
💲git remote set-url origin https://github.com/username/MyRepo.git  
```

#### <font color="#00FFFF">📑➒- It's good practice to first create all necessary branches and files on github and then clone it to your local repo:</font>  


```python
💲git clone https://github.com/username/MyRepo.git 
```

Alternatively if you have a local repository full of work; you can push it to online repo on GitHub.  
push our master branch to the origin url, and set it as the default remote branch:


```python
💲git push --set-upstream origin master
```

#### <font color="#00FFFF">⇄➓- Then Create parallel branches in local repository:</font>    
**💾for example if your github repository has branches called:**  
   **<font color="green">main, firs_branch, second_branch</font>**   
      **<font color="brown">💾create the same local branches:</font>**


```python
💲git checkout -b main  # if it's not created when cloning!  
💲git checkout -b first_branch  
💲git checkout -b second_branch  
```

**<font color="brown"> 🕎 to change branches and move between them:👇</font>** 


```python
💲git checkout `branch_name` 
```

**<font color="brown">👀 to check which branch are you currently in and to see which files are or are not in staging area👇</font>** 


```python
💲git status
`git status --short` #to see the changes in a more compact way!
output:  M index.html
Note: Short status flags are:   

?? - Untracked files  
A - Files added to stage  
M - Modified files  
D - Deleted files  
```

#### <font color="#00FFFF">➕➊➊- To add a file to a branch; got to that branch,first pull from online branch, then add and push to it:</font>   


```python
💲git checkout `branch_name`  
💲git pull origin `branch_name`
```

**<font color="brown">🔄to discard changes in working directory👇</font>**  


```python
💲git checkout -- filename 
```

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head4">🌀git workflow🌀</a></font>

### <font color="#00FFFF">1- Modify a file:</font>


```python
💲nano filename #👆🏾save and exit(ctrl+o,   ENTER, ctrl+x)
💲echo "lines to append" >> filename
```

### <font color="#00FFFF">2- Save the draft to Staging area:</font>


```python
💲git add filename
# 👆🏾add the given file
💲git add . # also `git add -A` or `git add --all`
#👆🏾add all files and directories in current location.
```

### <font color="#00FFFF">3- Commit the updated file:</font>


```python
💲git commit -m "log message goes here"
git commit -a -m "log message"  # commit directly, without adding the file to staging area; which is not recomended.
```

### <font color="#00FFFF">4- Repeat...</font>

Working with Files  
Adding and removing files  
Add a file or directory to git for tracking   
$ git add <filename_or_dir>  

Add all untracked and tracked files inside the current directory to git  
$ git add .  

Remove a file from a working directory or staging area  
$ git rm <<filename_or_dir>   
**One furthur step is pulling and pushing, if you are woriking with remote repo such as GitHub.
[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head5">🗃 Comparing Files 🗃</a></font>

#### <font color="#00FFFF">1- Compare the last commited version of a file with the <mark>unstaged version(draft)</mark>:</font>


```python
💲git diff filename
```

*<font color='green'>in the output, `a` is the saved(commited) version and `b` is the one that we have not added to the staging area.</font>*

#### <font color="#00FFFF">2- Compare a <mark>Staged</mark> file with the las commit:</font> 


```python
💲git diff -r HEAD filename
```

<font color='green'>🎯the flag `-r` stands for *particular <mark>revision</mark>* of the file.</font>  
<font color='green'>🎯`HEAD` is shortcut for the most recent commit. `-r` wont work without `HEAD`</font>

#### <font color="#00FFFF">3- Compare <mark>multiple staged</mark> files to the last commited version:</font>


```python
💲git diff -r HEAD
```

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head6">📑 Commit Structure (3 parts):</a></font>

### <font color="#00FFFF">🌀commit</font>  
#### <font color="green">contains metadata(author, commit message and time of the commit)</font>

##### <font color="brown">🦄 there is a unique identifier called `Hash`, composed of `40` character string of numbers and letters.</font>
**🦄Git produces it using pseudo-random number generator called <mark>Hash Function.</mark>**
*   ***🔖Hashes allow <mark>data sharing between repos.</mark>***
      > 🎯if two files are the same, then their hashes are the same.  
      > 🎯Git compare hashes rather than entire files.  
      > 🎯To compare, we only need the __<font color="orange">first 6-8 characters</font>__ of the hash.  
    >>💲`git log`  To view the history of commits for a repository  
    >>💲`git show c27fa856`  
          <blockquote> __🌊output:__  
             💧log entry at the top  
             💧diff output between `file in that commi` and `current version in the repo`  
             💧the last line is Data Entry Error  
      </blockquote>

### <font color="#00FFFF">🌀Tree:</font>  
   #### <font color="green">🎯It tracks the names and locations in the repo, when taht commit happened.</font>
***📂here we can see which files are modified.***

### <font color="#00FFFF">🌀Blob:</font>  
* #### <font color="green">🎯For each file listed in the tree, there is a <mark>blob(binary large object).</mark></font>

##### <font color="brown">📂it contains a compressed snapshot of the file contents(any data type) at the time of commit happen.</font>

📌**to see commit information, use this command:**   
* 💲`git log`                 
   - <font color="#20B2AA">🎯it will display all commits made to the repo in chronological oreder, __starting with the oldest.__ </font>       
        - 🎯it will show Hash, author, date and commit message.        
             🔲 <mark>press space to see more</mark>        
             🔲 <mark>pres q to return to terminal</mark>

**<font color="#808000">Additional methods for comparing commits</fot>** 
* 💲`git diff -r HEAD`   <font color="green"> 👈compares stagedfiles to the version in the last commit.</font>
* 💲`git diff -r HEAD~1` <font color="green"> 👈this is the path to the second most recent commit.</font>
* 💲`git diff -r HEAD~2` <font color="green"> 👈points to the commit before the second</font>

***<font color="brown">🗃 look at the changes made to files in a specific commit:</font>***
    
* 💲`git show HEAD~3` <font color="green"> 👈looks at the fourth most recent commit.</font>


***<font color="brown">🗃🗃 see changes between two commits:</font>***
    
* `💲git diff HEAD~3 HEAD~2`  ❚or❚ `💲git diff 35f4b4d 186398f` 👈<font color="green">compare fourth and third most recent commit</fot>  

***<font color="brown">☰ see changes per document by line(for example to see who mades the last change to each line of a file):</font>***  

* `💲git annotate filename`
   - <font color="#00FFFF">🎯the output: Hash, Author, Time, Line, Line content.</font>

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head7">⎌Undoing Changes before commit⎌:</a></font>

#### <font color="#808000">🌀Unstage files(remove from staging area):</font>
* **step1:Unstage**
   - 💲`git reset HEAD filename` 🎯<mark>to unstage one file.</mark>
   - 💲`git reset HEAD` 🎯<mark>to remove all files from staging area.</mark>
* **step2:Edit fiel👉**
  - 💲`nano filename`
* **step3:Restage file**
  - 💲`git add filename`
* **step4:commit**
  - 💲`git commit -m "loge message"`
        
#### <font color="#808000">🌀Undo Changes to an Unstaged file</font>  
* 💲`git checkout -- filename`
  - 🎯<mark>this, reverses the file back to the version in the **last commit**.</mark>
       - <font color="#1D8348">⭐checkout⭐ means switching to a different version'.</font>
         
#### <font color="#808000">🌀Undo Changes to all Unstaged files in the current directory</font>
* 💲`git checkout .` 🎯<mark>dot refers to current directory</mark>
  - <font color="#1D8348">🔺this command must be run in the main directory in order to work❗</font>
             
#### <font color="#808000">🌀Unstaging & Undoing all files</font>
*    💲`git reset HEAD`   
*    💲`git checkout .`   
*    💲`git add .`   
*    💲`git commit -m "log message"`   

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head8">🔄Restoring and Reverting🔄</a></font>

* 💲`git log`👇
  - 🎯<font color="#008080">find the commit we want to revert to.</font>
* 💲`git log -3`👇
   - 🎯<font color="#008080">restrict number of commits(e.g.:shows the 3 most recent commits of all files.)</font>
* 💲`git log -3 filename`👇
   - <font color="#008080">⦿only look at the commit history of 1 file.</font>
* 💲`git log --since='Apr 2 2022'`👇
   - <font color="#008080">🗓 to restrict log by date(e.g.:commits since 2nd April 2022)</font>
* 💲`git log --since='Apr 2 2022' --until='Apr 11 2022'`👇
  - 🎯<font color="#008080">Commits between 2nd and 11th of April</font>
  
#### <font color="808000">🌀Restoring an old version of a file:</font>
> 1. 💲`git log --since='Apr 3 2019'` 🎯<font color="#008080">find the commit we need to restore file version to.</font>   
> -  💲`git checkout -- filename` 🎯<font color="#008080">revert version of a file in the last commit .</font>   
> 2-1. 💲`git checkout dc9d8fac filename` 🎯<font color="#008080">replace two dashes with `hash` to revert to a version from a <mark>specific commit</mark>.</font>
> 2-2. 💲`git checkout HEAD~1 filename` 🎯<font color="#008080">this is anoter approach, because it is the <mark>second to last commit</mark>.</font>

#### <font color="808000">🌀Restoring a repo(all files) to previous state:</font> 
> - 💲`git checkout dc9d8fac` or `git checkout HEAD~1` 🎯<font color="#008080">use the previous commands but ommit the file name</mark>.</font>

#### <font color="808000">🌀Clean a repository(delete files that are not currently being tracked:</font> 
> 1. 💲`git clean -n` 🎯<font color="#008080">to list all untracked files</mark>.</font>
> 2. 💲`git clean -f` 🎯<font color="#008080">to delete those files. <mark>be aware</mark>❗: by executing this command, the files are <font color="#FF0000">gone for good!</font></mark></font>

=-=-=-
Reversing changes
Checking out (switching to) older commits
$ git checkout HEAD~3

Checks out the third-to-last commit.
$ git checkout <commit_id>

Undo the latest commit but leave the working directory unchanged
$ git reset HEAD~1

You can undo as many commits as you want by changing the number after the tilde.

Discard all changes of the latest commit (no easy recovery)
$ git reset --hard HEAD~1

Instead of HEAD~n, you can provide commit hash as well. Changes after that commit will be destroyed.

Undo a single given commit, without modifying commits that come after it (a safe reset)
$ git revert [commit_id]

May result in revert conflicts

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head9">🔧Configuring Git🔧</a></font>

### <font color="#C71585">some tips and tricks to improve our workflow</font>
💲`git config --list` 🎯 <font color="#008080">access a list of customizable settings</font>  
**Git has 3 levels of settings, in order:**
> 💲`git config --local`  🎯 <font color="#008080">shows settings for one specific project.
>> <font color="#00CED1">***output:***  <mark>  __user.name & user.email__(two global settings), core.editor=nano, core.filemode=true</mark>...</font>
>
> 💲`git config --global` 🎯 <font color="#008080">shows settings for all of our projects.
>> 💲`git config --global user.name 'Pirikli Artan'` 🎯<font color="#008080"> example of modifying a global setting
>>> 🔴<font color="red"> If your username has a space, you have to wrap it in single quotation marks (' '), otherwise, Git will ignore anything after the space!</font>
>   
> 💲`git config --system` 🎯 <font color="#008080">displays settings for every users on this computer.</font>   

**Using alias(through global settings) to speedup our workflow(tipically shorten a command):**     
>💲`git config --global alias.ci 'commit -m'` 🎯 <font color="#008080">replacing `commit -m` with `ci`</font>     
>💲`git ci "log message goes here"` 🎯 <font color="#008080">now we can commit files using the alias `ci`</font>    
>💲`git config --global alias.unstage 'reset HEAD'` 🎯 <font color="#008080">replace `reset HEAD` with the alias`unstage`</font>
>> 🔴 <font color="red">Be careful not to overwrite any Git or Shell commands with your alias!</font>
>
> 🗃 <font color="#0000FF">Git stores your alias in a file called `.gitconfig`</font>   
>> 💲`git config --global --list` 🎯<font color="#008080">to access the <mark>.gitconfig</mark> file.</font>    
>> <font color="#00CED1">output format: <mark>alias.aliasname=command</mark>: `alias.ci= commit -m`

**Ignoring specific files:**    
> 💲`nano .gitignore`  🎯<font color="#008080"> create the file .gitignore in the root directory of your repository.</font>    
> **Inside the file**, for example:
>  `*.log` 🎯<font color="#008080"> <mark>The wildcar, asterisk, </mark> means Git will ignore any files ending with `.log` </font>    
> **commonly ignored files include:**  APIs, credentials, system files, software dependencies.

=-=-=-
Logging and reviewing work
List all commits with their author, commit ID, date, and message 
$ git log

List one commit per line (-n tag can be used to limit the number of commits displayed (e.g. -5))
$ git log --oneline [-n]

Log all commits with diff information
$ git log --stat

Log commits after some date (A sample value can be 4th of October, 2020 - “2020-10-04” or keywords such as “yesterday”, “last month”, etc. )
$ git log --oneline --after=”YYYY-MM-DD”

Log commits before some date (Both --after and --before tags can be used for date ranges)
$ git log --oneline --before=”last year”

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head9">⸙Branches𝌎</a></font>

## <font color="#4B0082">Git uses branches to systematically track multiple version of files.</font>   
### to bring branches back together, we merge them. 
Branches are special “copies” of the code base which allow you to work on different parts of a project and new features in an isolated environment.    
Changes made to the files in a branch won’t affect the “main branch” which is the main project   development channel.   
#### when merging two branches, the commits are called 'parent commit'.    
**`source` the branch we want to merge from.**    
**`destination` the branch we watnt to merge into.**
##### Benefits of branches:
> Avoiding endless subdirectories   
> Multiple user can work simultaneously   
> Everything is tracked.
> Minimizes the risk of conflicting versions.

`git branch` shows the existing branches
> in the output: the branch which has asterisk(*) next to it, is the branch which we are currently in.
   
`git checkout -b newbranch` to create new branch called newbranch.    

`git diff main newbranch` to see difference between two branches   

## Working with branches     
`git checkout newbranch` to switch to the newbranch   
`git branch` to check and verify if you are in the branch(the current branch has asterisk * next to it)  
### Why do we merge branches?    
`main`= ground truth
each branch should be for a specific task   
once the task is complete we should merge our change into main.   
to keep it up to date and accurate.   
`git merge sourche-branch destination-branch` to merge two branches  

-=--=
Branches
List all branches
$ git branch

$ git branch --list

$ git branch -a  (shows remote branches as well)

Create a new local branch named new_branch without checking out that branch
$ git branch <new_branch>

Switch into an existing branch named <branch>
$ git checkout <branch>

Create a new local branch and switch into it
$ git checkout -b <new_branch>

Safe delete a local branch (prevents deleting unmerged changes)
$ git branch -d <branch>

Force delete a local branch (whether merged or unmerged)
$ git branch -D <branch>

Rename the current branch to <new_name>
$ git branch -m <new_name>



[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# <font color="purple"><a id="head10">Handling Conflicts</a></font>

A conflict occurs when a file in different branches has different contents that prevent them from automatically merging into a single version.    

`git merge update main`
> output:    
> CONFLICT (add/add): Merge conflict in todo.txt  
> Auto merging todo.txt     
> Automatic merge failed; fix conflicts and then commit the results.

`nano todo.txt` to modify the file and solve conflict   
`git add todo.txt`   
`git commit -m "Resolving todo.txt conflict"`   
`git merge update main`   

**How to avoid conflicts?**  Prevention is better than cure!  
- use each brach for specific task.
- Avoid editing a same file in multiple branches.

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# Creating repos

A repository or a repo is any location that stores code and the necessary files that allow it to run without errors    
`git init project-name` to create new repository for our project.   
`cd project-name` to change directory to newly created one.     
`git status` to check if git repo  has initialized correctly.  
**Converting a project to git repo**   
`cd directory-name` to go to the existing project's directory.   
`git init` to convert it to a git repo.  
output: Initialized empty git repository in /home/user/directory-name/.git/   
`git status` to check the newly created repos status.   
**Caution:** Don't create git repo inside another git repo(nested repos).  
because there will be two .git directories.
when trying to make commits, git will get confused about which directory it needs to update.   

Creating local repositories    
Clone a repository from remote hosts (GitHub, GitLab, DagsHub, etc.)  
$ git clone <remote_repo_url>   

Initialize git tracking inside the current directory    
$ git init   

Create a git-tracked repository inside a new directory   
$ git init [dir_name]   

Clone only a specific branch   
$ git clone -branch <branch_name> <repo_url>   

Cloning into a specified directory    
$ git clone <repo_url> <dir_name>   

A note on cloning   
There are two primary methods of cloning a repository - HTTPS syntax and SSH syntax. While SSH cloning is generally considered a bit more secure because you have to use an SSH key for authentication, HTTPS cloning is much simpler and the recommended cloning option by GitHub.  

HTTPS   
$ git clone https://github.com/your_username/repo_name.git   

SSH   
$ git clone git@github.com:user_name/repo_name.git  

[🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝🔝](#top)

# Working with remotes   


A remote repo is a repo stored in the cloud through an online repo hosting service such as GitHub.   
We can copy existing remotes to our local computer by cloning them   
`git clone path-to-project-directory`
`git clone /home/piriklinux/LearNotes` clone a local repo.     
`git clone /home/piriklinux/LearNotes NewLearNotes` give a cloned repo a name.  
`git clone [URL]` to clone a remote repository from GitHub, Gitbucket or Gitlab...   
`git clone https://github.com/pirikli/LearNotes` colne the 'LearNotes' repository from GitHub.   
when cloning a repo, Git remembers where the original repo was.  It does this by storing a remote tag in the new repo's configuration. If we are in a repo, we can list the names of its remotes using git remote.    
`git remote`  list the names of its remotes using git remote.
`git remote -v` to get more information, such as remotes URLs.     

When cloning, Git will automatically name the remote as `origin`. We can add more remotes by specifying a name for Git to assign. We do this using the git remote add command, and provide two pieces of information - the name that we would like to assign to the remote repo, and the URL, or the path to the directory.       
`git remote add remote_name URL`   
`git remote add artan https://github.com/pirikli/myrepo`    
Here, we create a remote called Artan, which points to the url github-dot-com-slash-pirikli-slash-myrepo. It is useful to define the remote name as we can use it as a shortcut when merging rather than listing the URL or path.  


Managing remote repositories   
List remote repos  
$ git remote   

Create a new connection called <remote> to a remote repository on servers like GitHub, GitLab, DagsHub, etc.   
$ git remote add <remote> <url_to_remote>   

Remove a connection to a remote repo called <remote>  
$ git remote rm <remote>  

Rename a remote connection  
$ git remote rename <old_name> <new_name>  



=-=-==
Managing remote repositories
List remote repos
$ git remote

Create a new connection called <remote> to a remote repository on servers like GitHub, GitLab, DagsHub, etc.
$ git remote add <remote> <url_to_remote>

Remove a connection to a remote repo called <remote>
$ git remote rm <remote>

Rename a remote connection
$ git remote rename <old_name> <new_name>

Working with Files
Adding and removing files
Add a file or directory to git for tracking
$ git add <filename_or_dir>

Add all untracked and tracked files inside the current directory to git
$ git add .

Remove a file from a working directory or staging area
$ git rm <<filename_or_dir>

Saving and working with changes
See changes in the local repository
$ git status

Saving a snapshot of the staged changes with a custom message
$ git commit -m “[Commit message]”

Staging changes in all tracked files and committing with a message
$ git add -am “[Commit message]”

Editing the message of the latest commit
$ git commit --amend -m “[New commit message]”

Saving staged and unstaged changes to stash for a later use (see below for the explanation of a stash)
$ git stash

Stashing staged, unstaged and untracked files as well
$ git stash -u

Stashing everything (including ignored files)
$ git stash --all

Reapply previously stashed changes and empty the stash
$ git stash pop

Reapply previously stashed changes and keep the stash
$ git stash apply

Dropping changes in the stash
$ git stash drop

Show uncommitted changes since the last commit
$ git diff

Show the differences between two commits (should provide the commit IDs)
$ git diff <id_1> <id_2>

A note on stashes
Git stash allows you to temporarily save edits you've made to your working copy so you can return to your work later. Stashing is especially useful when you are not yet ready to commit changes you've done, but would like to revisit them at a later time. 
=-=-=-=-

# 🤲 Gathering from a remote📥

To compare the files in a remote against the contents of a local repo we first need to fetch versions from the remote  
on your local Git, fetch updates to see what has changed on GitHub:

`git fetch origin main`   origin is name of the romote repo, main is the main branch of local repo.   
`git fetch origin branch-name` fetch into a different branch. Here we fetch from the remote origin repo's `branch-name` branch.   

**Synchronizing content**

After fetching, we now have the contents of the remote in our local repo.  
However, we need to synchronize contents between the two repos.   
`git merge origin main`  perform a merge of the remote into the local repo's main branch, where we are currently located. 
Since the emergency-fix branch came directly from master, and no other changes had been made to master while we were working, Git sees this as a continuation of master. So it can "Fast-forward", just pointing both master and emergency-fix to the same commit.

**Pulling from a remote**
As the remote is the source of truth, it is often ahead of local repos, meaning the workflow of fetching content and  synchronizing locally is very common    
simplify the process of fetch and merge:   
`git pull origin main` agian the origin is the name of remote repo and main is the main branch of the local repo.   
**. Pulling with unsaved local changes**   
If we have been working locally and not yet committed our changes, then Git won't allow us to pull from a remote    
Run a command to find out the name(s) of remote repos linked to your project: `git remote -v`    
Gather contents from the remote origin repo into your local main branch: `git fetch origin main`      
Compare the remote repo with your local main branch(to see their difference): `git diff origin main`    
Use a single command to fetch and merge the origin repo into your local main branch: `git pull origin main`   


# Pushing to a remote   

Save changes locally first: add and commit.  
git push remote local_branch   push into remote from local branch.
Typical workflow is: pulling from remote, workin on files, save and commit, then pushing into remote.   
What happens if we don't start the workflow by pulling from the remote?   
`git push origin main`  
output:  .....
**Resolving the conflict**  
`git pull origin main` when trying to pull; Git automatically opens nano text editor and ask us to add a message for the merge.   
`git pull --no-edit origin main` to avoid providing a message.(this is not recomended!)   
`git push origin main` now you can push the changes...   
=-=--=-=-=
Push a copy of local branch named branch to the remote repo
$ git push <remote_repo> branch~

Delete a remote branch named branch (-d tag only works locally)
$ git push <remote_repo> :branch

$ git push <remote_repo> --delete branch

Merging a branch into the main branch
$ git checkout main

$ git merge <other_branch>

Merging a branch and creating a commit message
$ git merge --no-ff <other_branch>

Compare the differences between two branches
$ git diff <branch_1> <branch_2>

Compare a single <file> between two branches
$ git diff <branch_1> <branch_2> <file>

Pulling changes
Download all commits and branches from the <remote> without applying them on the local repo
$ git fetch <remote>

Only download the specified <branch> from the <remote>
$ git fetch <remote> <branch>

Merge the fetched changes if accepted
$ git merge <remote>/<branch>  
Get all the change history of the origin for this branch:  
git fetch origin    
Merge the current branch with the branch master, on origin:  
git merge origin/master  
A more aggressive version of fetch which calls fetch and merge simultaneously
$ git pull <remote>
Update the current branch from its origin using a single command   
git pull origin  

getting help for any git command:
`git command -help`
`git status -help` Show the possible options for the status command in command line  
`git command --help` open the relevant Git manual page  
`git help --all` l display a very long list of commands  


Remove the hello-you branch from the local repository:
`git branch -d hello-you`

push the current branch to its default remote origin:
git push origin
List all local and remote branches of the current Git.  
git branch -a  
List only remote branches of the current Git.  
git branch -r   



```python

```
