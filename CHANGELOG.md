# Execution commands in git Version
#####Admin@OMDALAVI MINGW64 ~
$ cd Build-a-Version-Controlled-DevOps-Project-with-Git/

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git
$ git init
Initialized empty Git repository in C:/Users/Admin/Build-a-Version-Controlled-DevOps-Project-with-Git/.git/

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (master)
$ git switch -c main
Switched to a new branch 'main'

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ echo "# My Awesome DevOps Project" > README.md

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git add README.md
warning: in the working copy of 'README.md', LF will be replaced by CRLF the next time Git touches it

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ ls
README.md  README.md~

####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ cat README.md
 My Awesome DevOps Project

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ cat README.md~

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ nano README.md

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ cat README.md
# My Awesome DevOps Project

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git commit -m "Initial commit: Add README.md"
[main (root-commit) 3654cdb] Initial commit: Add README.md
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git remote add origin https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git branch -M main

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push -u origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 265 bytes | 88.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git checkout -b dev
Switched to a new branch 'dev'

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (dev)
$ git push -u origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git/pull/new/dev
remote:
To https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

######Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (dev)
$ git checkout dev
Already on 'dev'
Your branch is up to date with 'origin/dev'.

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (dev)
$ git pull origin dev
From https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git
 * branch            dev        -> FETCH_HEAD
Already up to date.

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (dev)
$ git checkout -b feature/add-web-server
Switched to a new branch 'feature/add-web-server'

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ echo "Creating a simple web server..." > app.js
git add app.js
warning: in the working copy of 'app.js', LF will be replaced by CRLF the next time Git touches it

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ git add app.js
warning: in the working copy of 'app.js', LF will be replaced by CRLF the next time Git touches it

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ git commit -m "feat: Add initial web server file"
[feature/add-web-server f210749] feat: Add initial web server file
 1 file changed, 1 insertion(+)
 create mode 100644 app.js

#####Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ git push -u origin feature/add-web-server
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 330 bytes | 110.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote:
remote: Create a pull request for 'feature/add-web-server' on GitHub by visiting:
remote:      https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git/pull/new/feature/add-web-server
remote:
To https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git
 * [new branch]      feature/add-web-server -> feature/add-web-server
branch 'feature/add-web-server' set up to track 'origin/feature/add-web-server'.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ git init
Reinitialized existing Git repository in C:/Users/Admin/Build-a-Version-Controlled-DevOps-Project-with-Git/.git/

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ ls
README.md  README.md~  app.js

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (feature/add-web-server)
$ git switch main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ echo "# .gitignore File" > .gitignore

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ nano .gitignore

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ nano .gitignore

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git add .gitignore
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ gi commit -m "Initial commit: Add .gitignore"
[main 0d82be1] Initial commit: Add .gitignore
 1 file changed, 93 insertions(+)
 create mode 100644 .gitignore

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push -u origin main
To https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push -u origin .gitignore
fatal: invalid refspec '.gitignore'

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push -u origin main/.gitignore
fatal: invalid refspec 'main/.gitignore'

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git remote add origin https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git
error: remote origin already exists.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git pull origin main --rebase
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (7/7), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 3.03 KiB | 154.00 KiB/s, done.
From https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git
 * branch            main       -> FETCH_HEAD
   3654cdb..5ed55c2  main       -> origin/main
Successfully rebased and updated refs/heads/main.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push -u origin .gitignore
fatal: invalid refspec '.gitignore'

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 941 bytes | 313.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Omdalvi070205/Build-a-Version-Controlled-DevOps-Project-with-Git.git
   5ed55c2..98faadf  main -> main
branch 'main' set up to track 'origin/main'.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git add .gitignore

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git commit -m "Add .gitignore file"
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md~

nothing added to commit but untracked files present (use "git add" to track)

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push origin main
Everything up-to-date

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git checkout main
Already on 'main'
Your branch is up to date with 'origin/main'.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git merge dev
Already up to date.

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git tag -a v1.0.0 -m "Initial release with web server"

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push origin main
Everything up-to-date

Admin@OMDALAVI MINGW64 ~/Build-a-Version-Controlled-DevOps-Project-with-Git (main)
$ git push origin v1.0.0
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.

