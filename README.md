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


