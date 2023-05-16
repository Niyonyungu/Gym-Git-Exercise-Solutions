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
