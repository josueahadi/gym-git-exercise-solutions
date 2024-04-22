# GIT EXERCISES

## BUNDLE 1

### Exercise 1

```bash
ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS
$ mkdir gym-git-exercise-solutions

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS
$ cd gym-git-exercise-solutions/

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions
$ code .

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions
$ git init 
Initialized empty Git repository in C:/Users/ahadi/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions/.git/

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (master)
$ git branch -m master main

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ 

$ git add .

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git commit -m "initial commit"
[main (root-commit) a68ac66] initial commit
 1 file changed, 31 insertions(+)
 create mode 100644 README.md

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git remote add origin https://github.com/josueahadi/gym-git-exercise-solutions.git

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 447 bytes | 223.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/josueahadi/gym-git-exercise-solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")  

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git add README.md 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git commit -m "connected github repo with the project file"
[main e024fd3] connected github repo with the project file
 1 file changed, 31 insertions(+)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 866 bytes | 866.00 KiB/s, done.       
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)      
To https://github.com/josueahadi/gym-git-exercise-solutions.git
   a68ac66..e024fd3  main -> main

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git add .

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   README.md


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git commit "refactor: git history for previous commit"
error: pathspec 'refactor: git history for previous commit' did not match any file(s) known to git

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
[main 8f50b86] refactor: git history for previous commit
 1 file changed, 32 insertions(+), 2 deletions(-)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 658 bytes | 658.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/josueahadi/gym-git-exercise-solutions.git
   e024fd3..8f50b86  main -> main

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git branch
* dev
  main

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git checkout -b test
Switched to a new branch 'test'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git branch
  dev
  main
* test

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git add .

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git commit -m "new branches"
[test 0cd0c61] new branches
 2 files changed, 61 insertions(+)
 create mode 100644 index.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git push -u origin main
branch 'main' set up to track 'origin/main'.
Everything up-to-date

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git push
fatal: The current branch test has no upstream branch.
To push the current branch and set the remote as upstream, use

upstream, see 'push.autoSetupRemote' in 'git help config'.


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git status
On branch test
nothing to commit, working tree clean

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (test)
$ git checkout dev
Switched to branch 'dev'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git status
On branch dev
nothing to commit, working tree clean

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git branch -d test
error: the branch 'test' is not fully merged
hint: If you are sure you want to delete it, run 'git branch -D test'
hint: Disable this message with "git config advice.forceDeleteBranch false"

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git merge test
Updating 8f50b86..0cd0c61
Fast-forward
 README.md  | 50 ++++++++++++++++++++++++++++++++++++++++++++++++++
 index.html | 11 +++++++++++
 2 files changed, 61 insertions(+)
 create mode 100644 index.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git branch -d test
Deleted branch test (was 0cd0c61).
```

### Exercise 2

```bash 
ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git branch
* dev
  main

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
No local changes to save

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
No local changes to save

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

nothing added to commit but untracked files present (use "git add" to track)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add about.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html
        team.html


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash list
stash@{0}: WIP on dev: 5ec5407 new branches
stash@{1}: WIP on dev: 5ec5407 new branches 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add home.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash list
stash@{0}: WIP on dev: 5ec5407 new branches
stash@{1}: WIP on dev: 5ec5407 new branches 
stash@{2}: WIP on dev: 5ec5407 new branches 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add team.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ stash list
bash: stash: command not found

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash list
stash@{0}: WIP on dev: 5ec5407 new branches
stash@{1}: WIP on dev: 5ec5407 new branches 
stash@{2}: WIP on dev: 5ec5407 new branches 
stash@{3}: WIP on dev: 5ec5407 new branches 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (1f26605327b00e2f6dbc8e294da6120d3ce6a399)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add team.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash list
stash@{0}: WIP on dev: 5ec5407 new branches
stash@{1}: WIP on dev: 5ec5407 new branches 
stash@{2}: WIP on dev: 5ec5407 new branches 
stash@{3}: WIP on dev: 5ec5407 new branches 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop stash@{2
error: stash@{2 is not a valid reference

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop stash@{2}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{2} (aad68fe5dec372145d72ef5fea3d7ae1d3f5ac0d)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (15ef5f72322ca3c40bebee849eb189a7cb7bc7df)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add team.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash 
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop restore
error: restore is not a valid reference

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop stash@{2}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
Dropped stash@{2} (8c57c6fe931b0cba24cd33e8aa7a509eab41f409)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop 
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Dropped refs/stash@{0} (153dfa553f80bfc3f33e2df8b55e4d0d5c9180d9)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add team.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5ec5407 new branches

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{1} (f3f3caf2eab00dd2dec3d9592f31519ee4f791f0)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git commit -m "bringing back home with git
 stash pop..."
[dev 46f111c] bringing back home with git stash pop...
 1 file changed, 11 insertions(+)
 create mode 100644 home.html

Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 494 bytes | 494.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/josueahadi/gym-git-exercise-solutions.git
   5ec5407..46f111c  dev -> dev

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ it commit -m "setup the home and about pag
e"
bash: it: command not found

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git commit -m "setup the home and about pa
ge"
[dev 5511f3f] setup the home and about page
 1 file changed, 11 insertions(+)
 create mode 100644 about.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git status
On branch dev
Your branch is ahead of 'origin/dev' by 1 commit.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

no changes added to commit (use "git add" and/or "git commit -a")

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash list

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash list

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git add team.html 

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git stash
Saved working directory and index state WIP on dev: 5511f3f setup the home and about page

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)      
$ git reset

```

## BUNDLE 2

### Exercise 1

```bash
ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/bundle-2)
$ git add .

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/bundle-2)
$ git commit -m "added services page"
[ft/bundle-2 96a5c5e] added services page
 1 file changed, 14 insertions(+)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use   

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.       


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/bundle-2)
$ git push --set-upstream origin ft/bundle-2 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 395 bytes | 131.00 KiB/s, done.     
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)    
git-exercise-solutions/pull/new/ft/bundle-2
remote:
To https://github.com/josueahadi/gym-git-exercise-solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

### Exercise 2

```bash
ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)
$ git pull
Updating 8f50b86..9589149
Fast-forward
 README.md  | 413 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 about.html |  11 ++
 home.html  |  11 ++
 index.html |  11 ++
 4 files changed, 446 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 index.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main)     
$ git pull
Updating 9589149..3bc4bf7
Fast-forward
 README.md     | 36 ++++++++++++++++++++++++++++++++++++
 services.html | 11 +++++++++++
 2 files changed, 47 insertions(+)
 create mode 100644 services.html


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git branch -b ft/service-redesign
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch     
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs        
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git branch -b ft/service-redesign
error: unknown switch `b'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch     
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs        
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git add .

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git commit -m "new changes to the service.html file"
[ft/service-redesign 796daae] new changes to the service.html file
 1 file changed, 1 insertion(+), 1 deletion(-)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git push --set-upstream origin ft/service-redesign 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 12 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 316 bytes | 158.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:      
remote:      https://github.com/josueahadi/gym-git-exercise-solutions/pull/new/ft/service-redesign
remote:
To https://github.com/josueahadi/gym-git-exercise-solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git diff

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git branch main
fatal: a branch named 'main' already exists

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git diff

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git diff index.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git diff service.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git checkout ft/service-redesign 
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git diff service.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git merge ft/service-redesign 
Updating 37a6b9e..796daae
Fast-forward
 service.html | 2 +-
 1 file changed, 1 insertion(+), 1 deletion(-)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (main) 
$ git diff



```

## BUNDLE 3

### Exercise 1

```bash 
.com>
Date:   Mon Apr 22 12:37:03 2024 +0100

    Merge pull request #3 from josueahadi/ft/service-redesign

    new changes to the service.html file

commit 796daae0b278d15d0a5d02343a74995bb0f8ff30 (origin/ft/service-redesign)        
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:50:02 2024 +0200

    new changes to the service.html file

commit 37a6b9e063b55611b7af912ae7947c29197a535d
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:41:25 2024 +0200

    new changes

commit 13753ee82ea9d42a7045f94108666a2b8de6078c
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:38:59 2024 +0200

    services.html -> service.html

commit 3bc4bf7307e62d5536573650c479c50fda9426f5
Merge: 9589149 4e419d7
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:34:46 2024 +0200

    Merge pull request #2 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 4e419d74f53e692619936198f39a4724b12335fc (origin/ft/bundle-2, ft/bundle-2)   
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:27:35 2024 +0200

    new changes

commit 01116ad8bad6b592f5c036c83036e89dd0c84d59
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:26:41 2024 +0200

    create a new file services.html

commit 9589149f032a1f29a85666f3049896909c40b938
Merge: 8f50b86 96a5c5e
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:23:26 2024 +0200

    Merge pull request #1 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 96a5c5ef264687aa9be624797d9e33ecf956599a
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:12:58 2024 +0200

    added services page

commit 098504a720029053ed1087ebb89149766d911fe6 (origin/dev, dev)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:58:08 2024 +0200

    added terminal history for git stash

commit 5511f3fe5a9bf5ca29e4f6b97cad550eaba85aa0
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:52:53 2024 +0200

    setup the home and about page

commit eb0e62fe3e51914b1403423f654bf8504944d347
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:46:24 2024 +0200

    git stash terminal history

commit 46f111c8dc9b6e20775c490c744900f0976c2bd1
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:43:57 2024 +0200

    bringing back home with git stash pop...

commit 5ec5407dbc5a3656d154c3878042aa9f324f191b
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:20:59 2024 +0200

    new branches

commit 0cd0c61db4d80d2ec055515583287af677754def
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:16:58 2024 +0200

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

commit e024fd3478a2bb1d8ab2b51fcb0af67156e062be
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 10:53:45 2024 +0200

...skipping...
commit 74e348c6ac8be693b6374726057d9532e42f6486 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:54:09 2024 +0200

    fear: add team page

commit 29590b1d1f51431bca01a5ef621421bacd0e6ae8 (origin/main, main, ft/service-redesign, ft/contact-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:43:58 2024 +0200

    conflict resolution

commit d3217617a9327edd6060c80ddea687faf8680612
Merge: a56ca8b 2b334de
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:12:13 2024 +0200

    Merge branch 'main' of https://github.com/josueahadi/gym-git-exercise-solutions 

commit a56ca8ba404c6df0712b9de037b55279e2c3ead8
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:11:44 2024 +0200

    README updated for Bundle 2 Exercises

commit 2b334de0e7b3ae5dcda052208dc73f3ffa0f8c59
Merge: 37a6b9e 796daae
Author: Habib Josue Ahadi <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:37:03 2024 +0100

    Merge pull request #3 from josueahadi/ft/service-redesign

    new changes to the service.html file

commit 796daae0b278d15d0a5d02343a74995bb0f8ff30 (origin/ft/service-redesign)        
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:50:02 2024 +0200

    new changes to the service.html file

commit 37a6b9e063b55611b7af912ae7947c29197a535d
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:41:25 2024 +0200

    new changes

commit 13753ee82ea9d42a7045f94108666a2b8de6078c
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:38:59 2024 +0200

    services.html -> service.html

commit 3bc4bf7307e62d5536573650c479c50fda9426f5
Merge: 9589149 4e419d7
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:34:46 2024 +0200

    Merge pull request #2 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 4e419d74f53e692619936198f39a4724b12335fc (origin/ft/bundle-2, ft/bundle-2)   
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:27:35 2024 +0200

    new changes

commit 01116ad8bad6b592f5c036c83036e89dd0c84d59
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:26:41 2024 +0200

    create a new file services.html

commit 9589149f032a1f29a85666f3049896909c40b938
Merge: 8f50b86 96a5c5e
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:23:26 2024 +0200

    Merge pull request #1 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 96a5c5ef264687aa9be624797d9e33ecf956599a
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:12:58 2024 +0200

    added services page

commit 098504a720029053ed1087ebb89149766d911fe6 (origin/dev, dev)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:58:08 2024 +0200

    added terminal history for git stash

commit 5511f3fe5a9bf5ca29e4f6b97cad550eaba85aa0
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:52:53 2024 +0200

    setup the home and about page

commit eb0e62fe3e51914b1403423f654bf8504944d347
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:46:24 2024 +0200

    git stash terminal history

commit 46f111c8dc9b6e20775c490c744900f0976c2bd1
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:43:57 2024 +0200

    bringing back home with git stash pop...

commit 5ec5407dbc5a3656d154c3878042aa9f324f191b
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:20:59 2024 +0200

    new branches

commit 0cd0c61db4d80d2ec055515583287af677754def
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:16:58 2024 +0200

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

commit e024fd3478a2bb1d8ab2b51fcb0af67156e062be
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 10:53:45 2024 +0200

...skipping...
commit 74e348c6ac8be693b6374726057d9532e42f6486 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:54:09 2024 +0200

    fear: add team page

commit 29590b1d1f51431bca01a5ef621421bacd0e6ae8 (origin/main, main, ft/service-redesign, ft/contact-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:43:58 2024 +0200

    conflict resolution

commit d3217617a9327edd6060c80ddea687faf8680612
Merge: a56ca8b 2b334de
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:12:13 2024 +0200

    Merge branch 'main' of https://github.com/josueahadi/gym-git-exercise-solutions

commit a56ca8ba404c6df0712b9de037b55279e2c3ead8
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:11:44 2024 +0200

    README updated for Bundle 2 Exercises

commit 2b334de0e7b3ae5dcda052208dc73f3ffa0f8c59
Merge: 37a6b9e 796daae
Author: Habib Josue Ahadi <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:37:03 2024 +0100

    Merge pull request #3 from josueahadi/ft/service-redesign

    new changes to the service.html file

commit 796daae0b278d15d0a5d02343a74995bb0f8ff30 (origin/ft/service-redesign)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:50:02 2024 +0200

    new changes to the service.html file

commit 37a6b9e063b55611b7af912ae7947c29197a535d
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:41:25 2024 +0200

    new changes

commit 13753ee82ea9d42a7045f94108666a2b8de6078c
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:38:59 2024 +0200

    services.html -> service.html

commit 3bc4bf7307e62d5536573650c479c50fda9426f5
Merge: 9589149 4e419d7
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:34:46 2024 +0200

    Merge pull request #2 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 4e419d74f53e692619936198f39a4724b12335fc (origin/ft/bundle-2, ft/bundle-2)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:27:35 2024 +0200

    new changes

commit 01116ad8bad6b592f5c036c83036e89dd0c84d59
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:26:41 2024 +0200

    create a new file services.html

commit 9589149f032a1f29a85666f3049896909c40b938
Merge: 8f50b86 96a5c5e
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:23:26 2024 +0200

    Merge pull request #1 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 96a5c5ef264687aa9be624797d9e33ecf956599a
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:12:58 2024 +0200

    added services page

commit 098504a720029053ed1087ebb89149766d911fe6 (origin/dev, dev)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:58:08 2024 +0200

    added terminal history for git stash

commit 5511f3fe5a9bf5ca29e4f6b97cad550eaba85aa0
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:52:53 2024 +0200

    setup the home and about page

commit eb0e62fe3e51914b1403423f654bf8504944d347
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:46:24 2024 +0200

    git stash terminal history

commit 46f111c8dc9b6e20775c490c744900f0976c2bd1
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:43:57 2024 +0200

    bringing back home with git stash pop...

commit 5ec5407dbc5a3656d154c3878042aa9f324f191b
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:20:59 2024 +0200

    new branches

commit 0cd0c61db4d80d2ec055515583287af677754def
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:16:58 2024 +0200

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

commit e024fd3478a2bb1d8ab2b51fcb0af67156e062be
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 10:53:45 2024 +0200

...skipping...
commit 74e348c6ac8be693b6374726057d9532e42f6486 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:54:09 2024 +0200

    fear: add team page

commit 29590b1d1f51431bca01a5ef621421bacd0e6ae8 (origin/main, main, ft/service-redesign, ft/contact-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:43:58 2024 +0200

    conflict resolution

commit d3217617a9327edd6060c80ddea687faf8680612
Merge: a56ca8b 2b334de
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:12:13 2024 +0200

    Merge branch 'main' of https://github.com/josueahadi/gym-git-exercise-solutions

commit a56ca8ba404c6df0712b9de037b55279e2c3ead8
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:11:44 2024 +0200

    README updated for Bundle 2 Exercises

commit 2b334de0e7b3ae5dcda052208dc73f3ffa0f8c59
Merge: 37a6b9e 796daae
Author: Habib Josue Ahadi <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:37:03 2024 +0100

    Merge pull request #3 from josueahadi/ft/service-redesign

    new changes to the service.html file

commit 796daae0b278d15d0a5d02343a74995bb0f8ff30 (origin/ft/service-redesign)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:50:02 2024 +0200

    new changes to the service.html file

commit 37a6b9e063b55611b7af912ae7947c29197a535d
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:41:25 2024 +0200

    new changes

commit 13753ee82ea9d42a7045f94108666a2b8de6078c
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:38:59 2024 +0200

    services.html -> service.html

commit 3bc4bf7307e62d5536573650c479c50fda9426f5
Merge: 9589149 4e419d7
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:34:46 2024 +0200

    Merge pull request #2 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 4e419d74f53e692619936198f39a4724b12335fc (origin/ft/bundle-2, ft/bundle-2)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:27:35 2024 +0200

    new changes

commit 01116ad8bad6b592f5c036c83036e89dd0c84d59
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:26:41 2024 +0200

    create a new file services.html

commit 9589149f032a1f29a85666f3049896909c40b938
Merge: 8f50b86 96a5c5e
Author: Angekarara <99403587+Angekarara@users.noreply.github.com>
Date:   Mon Apr 22 12:23:26 2024 +0200

    Merge pull request #1 from josueahadi/ft/bundle-2

    Ft/bundle 2

commit 96a5c5ef264687aa9be624797d9e33ecf956599a
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:12:58 2024 +0200

    added services page

commit 098504a720029053ed1087ebb89149766d911fe6 (origin/dev, dev)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:58:08 2024 +0200

    added terminal history for git stash

commit 5511f3fe5a9bf5ca29e4f6b97cad550eaba85aa0
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:52:53 2024 +0200

    setup the home and about page

commit eb0e62fe3e51914b1403423f654bf8504944d347
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:46:24 2024 +0200

    git stash terminal history

commit 46f111c8dc9b6e20775c490c744900f0976c2bd1
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:43:57 2024 +0200

    bringing back home with git stash pop...

commit 5ec5407dbc5a3656d154c3878042aa9f324f191b
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:20:59 2024 +0200

    new branches

commit 0cd0c61db4d80d2ec055515583287af677754def
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:16:58 2024 +0200

    new branches

commit 8f50b86dd8446a3cd3bed2157415fde31dde571e
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 11:07:19 2024 +0200

    refactor: git history for previous commit

commit e024fd3478a2bb1d8ab2b51fcb0af67156e062be
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 10:53:45 2024 +0200

    connected github repo with the project file

commit a68ac663694d868206fd6c2d6f927fc87594c5b2
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 10:45:33 2024 +0200

    initial commit

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/team-page)
$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git cherry-pick 74e348c6ac8be693b6374726057d9532e42f6486
[ft/contact-page 9528032] fear: add team page
 Date: Mon Apr 22 14:54:09 2024 +0200       
 2 files changed, 12 insertions(+), 204 deletions(-)
 create mode 100644 team.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git status
On branch ft/contact-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        contact.html

nothing added to commit but untracked files present (use "git add" to track)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git add --all

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git status
On branch ft/contact-page
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   contact.html


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git commit -m "feat: add contact page"
[ft/contact-page 63ae83c] feat: add contact page
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git status
On branch ft/contact-page
nothing to commit, working tree clean       

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 9, done.
Counting objects: 100% (9/9), done.
Delta compression using up to 12 threads    
Compressing objects: 100% (7/7), done.      
Writing objects: 100% (7/7), 902 bytes | 128.00 KiB/s, done.
Total 7 (delta 3), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (3/3), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/josueahadi/gym-git-exercise-solutions/pull/new/ft/contact-page
remote:
To https://github.com/josueahadi/gym-git-exercise-solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git commit -m "feat: add faq page"
On branch ft/faq-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        faq.html

nothing added to commit but untracked files present (use "git add" to track)

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git add --all

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git commit -m "feat: add faq page"
[ft/faq-page 46f5c21] feat: add faq page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 12 threads    
Compressing objects: 100% (3/3), done.      
Writing objects: 100% (3/3), 431 bytes | 107.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/josueahadi/gym-git-exercise-solutions/pull/new/ft/faq-page
remote:
To https://github.com/josueahadi/gym-git-exercise-solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
commit 46f5c21750c35621eb4db356bf496437a0520964 (HEAD -> ft/faq-page, origin/ft/faq-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 15:20:56 2024 +0200

    feat: add faq page

commit 63ae83cfe6e063dcf7fc0fa89fe7cd0f96d3042c (origin/ft/contact-page, ft/contact-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 15:10:01 2024 +0200

    feat: add contact page

commit 95280329f3305bf8b9e1f5fcc1093bac3854d196
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:54:09 2024 +0200

    fear: add team page

commit 29590b1d1f51431bca01a5ef621421bacd0e6ae8 (origin/main, main, ft/service-redesign)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:43:58 2024 +0200

    conflict resolution

commit d3217617a9327edd6060c80ddea687faf8680612
Merge: a56ca8b 2b334de
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:12:13 2024 +0200

    Merge branch 'main' of https://github.com/josueahadi/gym-git-exercise-solutions

commit a56ca8ba404c6df0712b9de037b55279e2c3ead8
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:11:44 2024 +0200

    README updated for Bundle 2 Exercises
e)
$ git revert 95280329f3305bf8b9e1f5fcc1093bac3854d196
[ft/faq-page f430e63] Revert "fear: add team page"
 2 files changed, 204 insertions(+), 12 deletions(-)
 delete mode 100644 team.html

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git status
On branch ft/faq-page
Your branch is ahead of 'origin/ft/faq-page' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
$ git log
commit f430e6317578a32ac1adf83033b8b0fc72c10c01 (HEAD -> ft/faq-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 15:23:14 2024 +0200

    Revert "fear: add team page"

    This reverts commit 95280329f3305bf8b9e1f5fcc1093bac3854d196.

commit 46f5c21750c35621eb4db356bf496437a0520964 (origin/ft/faq-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 15:20:56 2024 +0200

    feat: add faq page

commit 63ae83cfe6e063dcf7fc0fa89fe7cd0f96d3042c (origin/ft/contact-page, ft/contact-page)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 15:10:01 2024 +0200

    feat: add contact page

commit 95280329f3305bf8b9e1f5fcc1093bac3854d196
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:54:09 2024 +0200

    fear: add team page

commit 29590b1d1f51431bca01a5ef621421bacd0e6ae8 (origin/main, main, ft/service-redesign)
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:43:58 2024 +0200

    conflict resolution

commit d3217617a9327edd6060c80ddea687faf8680612
Merge: a56ca8b 2b334de
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:12:13 2024 +0200

    Merge branch 'main' of https://github.com/josueahadi/gym-git-exercise-solutions

commit a56ca8ba404c6df0712b9de037b55279e2c3ead8
Author: Josue <ahadihjosue@gmail.com>
Date:   Mon Apr 22 14:11:44 2024 +0200

    README updated for Bundle 2 Exercises

commit 2b334de0e7b3ae5dcda052208dc73f3ffa0f8c59
Merge: 37a6b9e 796daae
Author: Habib Josue Ahadi <ahadihjosue@gmail.com>
Date:   Mon Apr 22 12:37:03 2024 +0100

    Merge pull request #3 from josueahadi/ft/service-redesign

    new changes to the service.html file


ahadi@windows MINGW64 ~/OneDrive/Desktop/PROJECTS/gym-git-exercise-solutions (ft/faq-page)
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/josueahadi/gym-git-exercise-solutions.git
   46f5c21..f430e63  ft/faq-page -> ft/faq-page

```
