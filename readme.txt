GIT Commands:
git config --list 	-	List configurations
git help <verb>		-	Help command for any verb
git clone <URL>	<Optional Library Name>		-		clones remote repository from URL to local machine
git init	-	Initialize git repository
git status	-	Status of git repository
git diff	-	Shows what you changed but not staged
git diff --staged	-	shows what you have staged that will go into your commit
git add <file/folder name>	-	to begin stacking new files, stage changed files before commit
git add .	-	stage all files
git add *.html	-	Wildcard staging. Stage all html files. 

git reset HEAD <file>	-	Unstage already staged <file>
git checkout --<file/folder>	-	Discards changes made in local file/folder and retrieves latest code from git
git commit	-	press i, type message, press 'ESC', type :wq
git commit -m '<Comment>'	-	can type comment in the command line itself
git commit -a 	-	Git automatically stages every file that is already tracked before doing a commit
git commit --amend	-	can be used if commited too early and forgot to stage few files. This commit replace the original commit

git rm <filename>	-	stages file to be removed from git tracking. Next commit will delete the file from branch and also from you working directory
git rm --cached <filename>	-	removes file from staging area. Useful if something is staged by mistake
git mv <Old_file_Name> <New_File_Name>	-	Renames file

git log		-	gives log of commits
git log -p 	-	shows difference introduced in each commit
git log -p -<n>	-	limits output to last n entries
git log --stat	-	shows logs with statistics of files changed
git log --since=2.weeks	-	shows logs since last two weeks
git log -S<String>	-	only shows commits that changed or removed <String>
Shift + Z + Z		-	 to come out of the editor


touch .gitignore	-	for creating .gitignore file which can be used for ignoring some files from being tracked in git
					-	add names of files that you want to ignore into this .gitignore file
					-	git status no longer shows files added to this list
					
git remote	-			lists current remote branches
git remote -v	-		shows URLs for remote		
git remote 	add <short Name> <URL>	-	TO add remote repository, can be used with short-name	
git remote show <branch_name>	-	gives information about the remote branch
git remote rename <Old_Referance>	<New_Referance>	-	Renames how you referance the branch
git remote rm <Branch_Name>	-	Removes the branch

git tag		- lists available tags(marked inportant points in history)
git tag -l 'v1.8*'	-	lists tags starting with v1.8 only
git tag <tag name>	-	Creates lightweight tag
git tag -a <tag name> -m 'message'	-	Creates annotated tag with name tag-name
git tag -1 <tag name> <SHAid or part of SHAid>	-	creates tag for commits made in history
git show <tag_name>	-	gives information about the tag
git push origin <tag name> or --tags	-	pushes tag-name or all tags to remote branch

	

git branch <BranchName>	-	Create a new branch
git checkout <BranchName>	-	switch to <BranchName>	master is the main branch
git commit -a -m '<comment>	-	skip staging step. Only files already being tracked will be considered, new files have to be added using staging command
git stash	-			park your changes without committing them if you need to switch to new branch
git stash apply -		pull back changes that you parked before

git fetch origin	-	gets any changes from source since you cloned or fetched but will not merge into your directory
git pull origin 	- fetches and merges into your directory
git push origin master	-	push to branch known as origin and merge into master branch
git remote add <BranchName> <URL>	-	create remote branch by name <BranchName> at <URL>

