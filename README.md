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



```