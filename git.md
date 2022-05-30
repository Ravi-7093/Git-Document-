Git is software that keeps track of changes of files and directories 
Specially text changes  
Git – Version Control System (VCS) 
Source Code Management Tool also called. 
 
History  
Source Code Control System-1972  
Bundled with Linux –Developed by At and T 
It worked in such way that only changes were updated in each version the original remained as it is . 
 
Revision Control System – Cross Platform 
Faster – open source  
Stored the latest version if needed previous version apply snapshots 
 
Only single changes were handled (one singled file ). 
 
Concurrent Version System 
--open source 
--Multiple Files , --Multi User Repositories 
--Store code – called Code Repository --  
  put it in remote server – multi users could work simultaneously . 
 
SVN (Apache Subversion) 
 
--open source 
--faster  
--svn allowed tracking of text and images 
--svn not only tracks the changes done in the file but also the complete directory. 
 
BitKeeper SCM 
 
--2000 closed source , propriteary 
--closed source  
--contraversial  since it ran on linux but was not free 
 
Git  
--Linus travolds 
--Distributed version Control 
--Compatible with linux and Mac Os, Windows. 
--better safe guards for data protection 
 
 
Distributed Version Control  
 
--no need to communicate with server 
--no n\w is needed. 
--Encourage participate and work group project 

Git config --global config.name "value"

Man ls --git manual
Man git-log ---manual for the commands

Git init --initialize the repository

Git add .- points to the current directory

Creating Commit:
	1) Make Changes
	2) Add the Changes -- git add . 
	3) Commit changes to the repository with a message -- git commit -m " Msg"
	
Writing Commit Message:
	1) Start with issue id - ghi123 -"Short Description"
	2) Description

View Commit Log:
Git log -- checks the log file
Git log -n 5 -- limiting the commit log to the latest 5 commits
git log --since=2019-01-01 -- get the commits since the date mentioned 
Git log --grep ="Init" -- global regular expression --for searching the message value


Git repository --- after staging we put into git repo --git commit
Staging index -- after git add filename is pushed to staging index from working 
Working -- current file changes version 

Git creates checksum --uses SHA 1 to create checksums
It’s the hash value used to label one of the commits


HEAD - Pointer points to the current repository -reference variable
Points to the parent of next commit where writing commit takes place .

Git diff - to check the difference in the contents of the file b/w working and staging

--staging directory 
--working directory -If changes are made then its shown as +++ if new lines are added.

--If old lines are changed .

If we want to see the diff in contents in the file at the staging directory -- 
Git diff --staged ( diff repo and staging)

Delete Files:
Git -rm filename -- (at staging level)
Git commit -m "" -- so changes gets reflected at repository level

Move and rename files:
Git mv file_name (exists) file_name_2(new file)

Git Commit -a :
Commits all the files from working to repository
Does not include untracked files

 git diff --color-words -- to check the exact change 

 git show f78ac0 -- check the commit and its changes (actually what happened)

git diff d38c64..HEAD --color-words -- compares the changes made in the commits made 

Git log --online -- gives the one line of the commit message 

Git atomic commits
Git add -filename

Git restore filename -- restores the older version in the working directory

Git reset HEAD filename -- to get the changed  files  from staging index back to working directory.

git commit --amend -m " " -- to overwrite the old commit and add new commit

Git ammends only restore the most commit.

Git checkout commit value -- filename

Git diff -- staged

Git revert - reverting to the old commit

Git clean -n -- for listing files for cleaning untracked files
Git clean -f -- for deleting files 

Since the HEAD points to the repository's current version of files, Git will reset the footer.css in the staging index with the repository version of footer.css.
git reset HEAD footer.css

git clean -f -- force clean

git checkout replaces the working directory version of a file with the repository version of the file, so the committed file is the version that will be checked out.

