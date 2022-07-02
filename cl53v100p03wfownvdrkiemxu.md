## Git and GitHub Command Cheat Sheet

##### Table of Contents Hide

1.  [The essential Git commands every developer must know](https://blog.aldinn.com/#the-essential-git-commands-every-developer-must-know)

2.  [Creating Snapshots‌](https://blog.aldinn.com/#creating-snapshots)
    1.  1.  1.  [Initializing a repository](https://blog.aldinn.com/#initializing-a-repository)
            2.  [Staging files](https://blog.aldinn.com/#staging-files)
            3.  [Viewing the status](https://blog.aldinn.com/#viewing-the-status)
            4.  [Committing the staged files](https://blog.aldinn.com/#committing-the-staged-files)
            5.  [Skipping the staging area](https://blog.aldinn.com/#skipping-the-staging-area)
            6.  [Removing files](https://blog.aldinn.com/#removing-files)
            7.  [Renaming or moving files](https://blog.aldinn.com/#renaming-or-moving-files)
            8.  [Viewing the staged/unstaged changes](https://blog.aldinn.com/#viewing-the-staged-unstaged-changes)
            9.  [Viewing the history](https://blog.aldinn.com/#viewing-the-history)
            10.  [Viewing a commit](https://blog.aldinn.com/#viewing-a-commit)
            11.  [Unstaging files (undoing git add)](https://blog.aldinn.com/#unstaging-files-undoing-git-add)
            12.  [Discarding local changes](https://blog.aldinn.com/#discarding-local-changes)
            13.  [Restoring an earlier version of a file](https://blog.aldinn.com/#restoring-an-earlier-version-of-a-file)
3.  [Browsing History‌](https://blog.aldinn.com/#browsing-history)
    1.  1.  1.  [Viewing the history](https://blog.aldinn.com/#viewing-the-history-2)
            2.  [Filtering the history](https://blog.aldinn.com/#filtering-the-history)
            3.  [Formatting the log output](https://blog.aldinn.com/#formatting-the-log-output)
            4.  [Creating an alias](https://blog.aldinn.com/#creating-an-alias)
            5.  [Viewing a commit](https://blog.aldinn.com/#viewing-a-commit-2)
            6.  [Comparing commits](https://blog.aldinn.com/#comparing-commits)
            7.  [Checking out a commit](https://blog.aldinn.com/#checking-out-a-commit)
            8.  [Finding a bad commit](https://blog.aldinn.com/#finding-a-bad-commit)
            9.  [Finding contributors](https://blog.aldinn.com/#finding-contributors)
            10.  [Viewing the history of a file](https://blog.aldinn.com/#viewing-the-history-of-a-file)
            11.  [Finding the author of lines](https://blog.aldinn.com/#finding-the-author-of-lines)
            12.  [Tagging](https://blog.aldinn.com/#tagging)
4.  [Branching & Merging‌](https://blog.aldinn.com/#branching-merging)
    1.  1.  1.  [Managing branches](https://blog.aldinn.com/#managing-branches)
            2.  [Comparing branches](https://blog.aldinn.com/#comparing-branches)
            3.  [Stashing](https://blog.aldinn.com/#stashing)
            4.  [Merging](https://blog.aldinn.com/#merging)
            5.  [Viewing the merged branches](https://blog.aldinn.com/#viewing-the-merged-branches)
            6.  [Rebasing](https://blog.aldinn.com/#rebasing)
            7.  [Cherry picking](https://blog.aldinn.com/#cherry-picking)
5.  [Collaboration‌](https://blog.aldinn.com/#collaboration)
    1.  1.  1.  [Cloning a repository](https://blog.aldinn.com/#cloning-a-repository)
            2.  [Syncing with remotes](https://blog.aldinn.com/#syncing-with-remotes)
            3.  [Sharing tags](https://blog.aldinn.com/#sharing-tags)
            4.  [Sharing branches](https://blog.aldinn.com/#sharing-branches)
            5.  [Managing remotes](https://blog.aldinn.com/#managing-remotes)
6.  [Rewriting History‌](https://blog.aldinn.com/#rewriting-history)
    1.  1.  1.  [Undoing commits](https://blog.aldinn.com/#undoing-commits)
            2.  [Reverting commits](https://blog.aldinn.com/#reverting-commits)
            3.  [Recovering lost commits](https://blog.aldinn.com/#recovering-lost-commits)
            4.  [Amending the last commit](https://blog.aldinn.com/#amending-the-last-commit)
            5.  [Interactive rebasing](https://blog.aldinn.com/#interactive-rebasing)

The essential Git commands every developer must know
----------------------------------------------------

This cheat sheet covers all of the Git commands I’ve covered in my Ultimate Git  
Mastery blog.  
✓ Creating snapshots  
✓ Browsing history  
✓ Branching & merging  
✓ Collaboration using Git & GitHub  
✓ Rewriting history

Creating Snapshots‌
===================

#### Initializing a repository

    git init 

#### Staging files

    git add file1.js 
    # Stages a single file 

    git add file1.js file2.js
    # Stages multiple files 

    git add *.js 
    # Stages with a pattern

    git add . 
    # Stages the current directory and all its content

#### Viewing the status

    git status 
    # Full status

    git status -s 
    # Short status

#### Committing the staged files

    git commit -m “Message” 
    # Commits with a one-line message

    git commit 
    # Opens the default editor to type a long message

#### Skipping the staging area

    git commit -am “Message”

#### Removing files

    git rm file1.js 
    # Removes from working directory and staging area 

    git rm --cached file1.js 
    # Removes from staging area only

#### Renaming or moving files

    git mv file1.js file1.txt

#### Viewing the staged/unstaged changes

    git diff 
    # Shows unstaged changes

    git diff --staged 
    # Shows staged changes

    git diff --cached 
    # Same as the above

#### Viewing the history

    git log 
    # Full history

    git log --oneline 
    # Summary

    git log --reverse 
    # Lists the commits from the oldest to the newest

#### Viewing a commit

    git show 921a2ff 
    # Shows the given commit

    git show HEAD 
    # Shows the last commit

    git show HEAD~2 
    # Two steps before the last commit

    git show HEAD:file.js 
    # Shows the version of file.js stored in the last commit

#### Unstaging files (undoing git add)

    git restore --staged file.js 
    # Copies the last version of file.js from repo to index

#### Discarding local changes

    git restore file.js 
    # Copies file.js from index to working directory 
    

    git restore file1.js file2.js 
    # Restores multiple files in working directory

    git restore . 
    # Discards all local changes (except untracked files) 

    git clean -fd 
    # Removes all untracked files

#### Restoring an earlier version of a file

    git restore --source=HEAD~2 file.js

Browsing History‌
=================

#### Viewing the history

    git log --stat 
    # Shows the list of modified files

    git log --patch 
    # Shows the actual changes (patches)

#### Filtering the history

    git log -3 
    # Shows the last 3 entries

    git log --author=“Mosh”

    git log --before=“2020-08-17”

    git log --after=“one week ago”

    git log --grep=“GUI” 
    # Commits with “GUI” in their message

    git log -S“GUI” 
    # Commits with “GUI” in their patches 

    git log hash1..hash2 
    # Range of commits

    
    git log hash1..hash2 
    # Range of commits

    git log file.txt 
    # Commits that touched file.txt

#### Formatting the log output

    git log --pretty=format:”%an committed %H”

#### Creating an alias

    git config --global alias.lg “log --oneline"

#### Viewing a commit

    git show HEAD~2

    git show HEAD~2:file1.txt 
    # Shows the version of file stored in this commit

#### Comparing commits

    git diff HEAD~2 HEAD 
    # Shows the changes between two commits 

    git diff HEAD~2 HEAD file.txt 
    # Changes to file.txt only

#### Checking out a commit

    git checkout dad47ed 
    # Checks out the given commit 

    git checkout master
    # Checks out the master branch

#### Finding a bad commit

    git bisect start

    git bisect bad 
    # Marks the current commit as a bad commit 

    git bisect good ca49180 
    # Marks the given commit as a good commit 

    git bisect reset 
    # Terminates the bisect session

#### Finding contributors

    git shortlog

#### Viewing the history of a file

    git log file.txt 
    # Shows the commits that touched file.txt

    git log --stat file.txt 
    # Shows statistics (the number of changes) for file.txt 

    git log --patch file.txt 
    # Shows the patches (changes) applied to file.txt

#### Finding the author of lines

    git blame file.txt 
    # Shows the author of each line in file.txt

#### Tagging

    git tag v1.0 
    # Tags the last commit as v1.0 

    git tag v1.0 5e7a828 
    # Tags an earlier commit

    git tag # Lists all the tags

    git tag -d v1.0 # Deletes the given tag

Branching & Merging‌
====================

#### Managing branches

    git branch bugfix 
    # Creates a new branch called bugfix 

    git checkout bugfix 
    # Switches to the bugfix branch

    git switch bugfix 
    # Same as the above 

    git switch -C bugfix 
    # Creates and switches

    git branch -d bugfix 
    # Deletes the bugfix branch

#### Comparing branches

    git log master..bugfix 
    # Lists the commits in the bugfix branch not in master 

    git diff master..bugfix 
    # Shows the summary of changes

#### Stashing

    git stash push -m “New tax rules” 
    # Creates a new stash 
    

    git stash list 
    # Lists all the stashes

    git stash show [email protected]{1} 
    # Shows the given stash

    git stash show 1 
    # shortcut for [email protected]{1}

    git stash apply 1 
    # Applies the given stash to the working dir

    git stash drop 1 
    # Deletes the given stash

    git stash clear 
    # Deletes all the stashes

#### Merging

    git merge bugfix 
    # Merges the bugfix branch into the current branch 

    git merge --no-ff bugfix 
    # Creates a merge commit even if FF is possible

    git merge --squash bugfix 
    # Performs a squash merge

    git merge --abort 
    # Aborts the merge

#### Viewing the merged branches

    git branch --merged 
    # Shows the merged branches 

    git branch --no-merged 
    # Shows the unmerged branches

#### Rebasing

    git rebase master 
    # Changes the base of the current branch

#### Cherry picking

    git cherry-pick dad47ed 
    # Applies the given commit on the current branch

Collaboration‌
==============

#### Cloning a repository

    git clone url

#### Syncing with remotes

    git fetch origin master 
    # Fetches master from origin 

    git fetch origin 
    # Fetches all objects from origin

    git fetch 
    # Shortcut for “git fetch origin”

    git fetch 
    # Shortcut for “git fetch origin”

    git pull 
    # Fetch + merge

    git push origin master 
    # Pushes master to origin

    git push 
    # Shortcut for “git push origin master”

#### Sharing tags

    git push origin v1.0 
    # Pushes tag v1.0 to origin 
    git push origin —delete v1.0

#### Sharing branches

    git branch -r 
    # Shows remote tracking branches

    git branch -vv 
    # Shows local & remote tracking branches 

    git push -u origin bugfix 
    # Pushes bugfix to origin

    git push -d origin bugfix 
    # Removes bugfix from origin

#### Managing remotes

    git remote 
    # Shows remote repos

    git remote add upstream url 
    # Adds a new remote called upstream 

    git remote rm upstream 
    # Remotes upstream

Rewriting History‌
==================

#### Undoing commits

    git reset --soft HEAD^ 
    # Removes the last commit, keeps changed staged 

    git reset --mixed HEAD^ 
    # Unstages the changes as well

    git reset --hard HEAD^ 
    # Discards local changes

#### Reverting commits

    git revert 72856ea 
    # Reverts the given commit

    git revert HEAD~3.. 
    # Reverts the last three commits 
    git revert --no-commit HEAD~3..

#### Recovering lost commits

    git reflog 
    # Shows the history of HEAD

    git reflog show bugfix 
    # Shows the history of bugfix pointer

#### Amending the last commit

    git commit --amend

#### Interactive rebasing

    git rebase -i HEAD~5

রিসোর্স সমুহ:

1.   [official Git project site](https://git-scm.com/) 
2.   [ProGit book](https://git-scm.com/book)
3.   [Git command list](https://git-scm.com/docs)
4.  [on-demand training courses](https://skills.github.com/)
5.  [on-demand training courses](https://skills.github.com/)
6.  [online Git course](https://www.pluralsight.com/courses/code-school-git-real)
7.  [git-cheat-sheet-education (github.com)](https://education.github.com/git-cheat-sheet-education.pdf)
8.  [Git cheat sheet | Atlassian Git Tutorial](https://www.atlassian.com/git/tutorials/atlassian-git-cheatsheet)

[What is git ?](https://blog.aldinn.com/what-is-git/)

[22](https://www.facebook.com/sharer.php?t=--SHARETEXT--&u=https://bit.ly/3mRUSPi)

[0](https://twitter.com/share?text=--SHARETEXT--&url=https://bit.ly/3mRUSPi)

[0](https://pinterest.com/pin/create/bookmarklet/?description=--SHARETEXT--&url=https://blog.aldinn.com/git-and-github-command-cheat-sheet/&media=https://res.cloudinary.com/aldinn/images/f_auto,q_auto/v1655332888/blog/Git-Github-6/Git-Github-6.png?_i=AA)

[0](https://blog.aldinn.com/cdn-cgi/l/email-protection#a59ad6d0c7cfc0c6d198e2ccd1809795c4cbc1809795e2ccd1edd0c7809795e6cac8c8c4cbc1809795e6cdc0c4d1809795f6cdc0c0d183c7cac1dc988888f6ede4f7e0f1e0fdf18888809795cdd1d1d5d69f8a8ac7ccd18bc9dc8a96c8f7f0f6f5cc)

[Share 22](https://www.facebook.com/sharer.php?t=--SHARETEXT--&u=https://bit.ly/3mRUSPi)

[Tweet 0](https://twitter.com/share?text=--SHARETEXT--&url=https://bit.ly/3mRUSPi)