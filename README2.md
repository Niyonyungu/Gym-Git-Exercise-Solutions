# GIT EXERCISE

## Bundle 5

### Exercise 1

```bash


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git pull
Already up to date.

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git add index.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   index.html

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    home.html


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git add home.html

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    home.html -> index.html


vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git commit -m "renamed homepage to index "
[main ca3aa1b] renamed homepage to index
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)

vainqueur@DESKTOP-KTN8E98 MINGW64 ~/Desktop/Git-exercises-solution (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 245 bytes | 245.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Niyonyungu/Gym-Git-Exercise-Solutions.git
   dd5020c..ca3aa1b  main -> main

vainq


```
