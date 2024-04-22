bundle 1:
exercise1:

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions
$ git init
Initialized empty Git repository in C:/Users/HP/Desktop/theGym/Gym Git Exercise Solutions/.git/

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (master)
$ git branch -m main

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git add index.html

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git commit -m "first commit"
[main (root-commit) c223cbc] first commit
 1 file changed, 15 insertions(+)
 create mode 100644 index.html

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git remote add origin https://github.com/emelyne1234/Gym-Git-Exercise-Solutions.git

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git pull origin main
From https://github.com/emelyne1234/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
fatal: refusing to merge unrelated histories

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git pull origin main --allow-unrelated-histories
From https://github.com/emelyne1234/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.
 README.md | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git push origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 715 bytes | 715.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/emelyne1234/Gym-Git-Exercise-Solutions.git
   2877821..6246112  main -> main

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git checkout -b test
Switched to a new branch 'test'

Lenovo@Emelyne MINGW64~/Desktop/theGym/Gym Git Exercise Solutions (test)
$ git checkout dev
Switched to branch 'dev'

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git branch -d test
Deleted branch test (was 6246112).


exercise2:
Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git add home.html

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 6246112 Merge branch 'main' of https://github.com/emelyne1234/Gym-Git-Exercise-Solutions

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git add about.html

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 6246112 Merge branch 'main' of https://github.com/emelyne1234/Gym-Git-Exercise-Solutions

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git add team.html

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: 6246112 Merge branch 'main' of https://github.com/emelyne1234/Gym-Git-Exercise-Solutions

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: 6246112 Merge branch 'main' of https://github.com/emelyne1234/Gym-Git-Exercise-Solutions
stash@{1}: WIP on dev: 6246112 Merge branch 'main' of https://github.com/emelyne1234/Gym-Git-Exercise-Solutions
stash@{2}: WIP on dev: 6246112 Merge branch 'main' of https://github.com/emelyne1234/Gym-Git-Exercise-Solutions

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (acedecb763ed1927ffb23dd78e5ae4cc3f02c558)

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (601b1b1024fbee80f343599753e082b5b13c9c01)

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git commit -m "about and team page were added"
[dev 6d99e82] about and team page were added
 2 files changed, 30 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git push origin
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 566 bytes | 566.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/emelyne1234/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/emelyne1234/Gym-Git-Exercise-Solutions.git
 * /[new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped stash@{0} (ad9317096c9a553ee968b24328643caa90800ac4)

Lenovo@Emelyne MINGW64 ~/Desktop/theGym/Gym Git Exercise Solutions (dev)
$ git reset --hard
HEAD is now at 6d99e82 about and team page were added



