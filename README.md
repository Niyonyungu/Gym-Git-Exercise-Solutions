# Git Exercise

## Bundle 1

### Exercise 1

```bash
vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution
$ git init
Initialized empty Git repository in C:/Users/vainqueur/Desktop/Git-exercises-solution/.git/

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (master)
$ code .

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (master)
$ git add README.md

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (master)
$ git commit -m "first commit"
[master (root-commit) fa4b404] first commit
 1 file changed, 5 insertions(+)
 create mode 100644 README.md

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (master)
$ git branch -M main

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git remote add origin https://github.com/Niyonyungu/Gym-Git-Exercise-Solutions.git

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 249 bytes | 249.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Niyonyungu/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git branch dev

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git checkout dev
Switched to branch 'dev'

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (dev)
$ git branch test

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (dev)
$ git branch
* dev
  main
  test

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (dev)
$ git branch --delete test
Deleted branch test (was f8d3a37).


```

### Exercise 2

```bash


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git add home.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash
Saved working directory and index state WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash list
stash@{0}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git add about.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash
Saved working directory and index state WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash list
stash@{0}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1
stash@{1}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git add team.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash
Saved working directory and index state WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash list
stash@{0}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1
stash@{1}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1
stash@{2}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (a7a0de19e378917523591d6da53088eaaceebe63)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash list
stash@{0}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1
stash@{1}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash pop stash@{1}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (66ec71dd34105fb61b64731aaf25e15cb2071d63)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git add --all

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git commit -m "about page and home page set up in exercise 2"
[main d021e92] about page and home page set up in exercise 2
 2 files changed, 30 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 572 bytes | 286.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/Niyonyungu/Gym-Git-Exercise-Solutions.git
   1012878..d021e92  main -> main

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash list
stash@{0}: WIP on main: 1012878 the updated readme file bundle 1 exercise 1

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git stash pop stash@{0}
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (b718fcf4741ec3babc9164e079385e51b5a0e304)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git reser --hard
git: 'reser' is not a git command. See 'git --help'.

The most similar commands are
        reset
        restore

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git reset --hard
HEAD is now at d021e92 about page and home page set up in exercise 2

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$


```
