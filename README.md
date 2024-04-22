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