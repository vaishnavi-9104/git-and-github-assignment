Microsoft Windows [Version 10.0.22621.3880]
(c) Microsoft Corporation. All rights reserved.

C:\Users\Dell>cd desktop

C:\Users\Dell\Desktop>cd demo

C:\Users\Dell\Desktop\demo>cd project

C:\Users\Dell\Desktop\demo\project>echo.> script.js

C:\Users\Dell\Desktop\demo\project>git init
Initialized empty Git repository in C:/Users/Dell/Desktop/demo/project/.git/

C:\Users\Dell\Desktop\demo\project>echo.> script.js

C:\Users\Dell\Desktop\demo\project>git add script.js

C:\Users\Dell\Desktop\demo\project>git commit -m "Add initial script.js with sayHello function"
[master (root-commit) 1093314] Add initial script.js with sayHello function
 1 file changed, 5 insertions(+)
 create mode 100644 script.js

C:\Users\Dell\Desktop\demo\project>git checkout -b feature-greeting
Switched to a new branch 'feature-greeting'

C:\Users\Dell\Desktop\demo\project>git checkout -b feature-greeting
fatal: a branch named 'feature-greeting' already exists

C:\Users\Dell\Desktop\demo\project>git add script.js

C:\Users\Dell\Desktop\demo\project>git commit -m "Add greetUser function for personalized greeting"
[feature-greeting 2a47060] Add greetUser function for personalized greeting
 1 file changed, 3 insertions(+)

C:\Users\Dell\Desktop\demo\project>git checkout main
error: pathspec 'main' did not match any file(s) known to git

C:\Users\Dell\Desktop\demo\project>git checkout master
Switched to branch 'master'

C:\Users\Dell\Desktop\demo\project>git merge feature-greeting
Updating 1093314..2a47060
Fast-forward
 script.js | 3 +++
 1 file changed, 3 insertions(+)

C:\Users\Dell\Desktop\demo\project>git remote add origin https://github.com/vaishnavi-9104/git-and-github-assignment.git

C:\Users\Dell\Desktop\demo\project>git branch -M main

C:\Users\Dell\Desktop\demo\project>git push -u origin main
remote: Invalid username or password.
fatal: Authentication failed for 'https://github.com/vaishnavi-9104/git-and-github-assignment.git/'

C:\Users\Dell\Desktop\demo\project>git remote add origin https://github.com/vaishnavi-9104/git-and-github-assignment.git
error: remote origin already exists.

C:\Users\Dell\Desktop\demo\project>git push -u origin master
error: src refspec master does not match any
error: failed to push some refs to 'https://github.com/vaishnavi-9104/git-and-github-assignment.git'

C:\Users\Dell\Desktop\demo\project>git push -u origin main
info: please complete authentication in your browser...

C:\Users\Dell\Desktop\demo\project>git remote add origin https://github.com/vaishnavi-9104/git-and-github-assignment.git
error: remote origin already exists.

C:\Users\Dell\Desktop\demo\project>git push -u origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (6/6), 597 bytes | 199.00 KiB/s, done.
Total 6 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/vaishnavi-9104/git-and-github-assignment.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

C:\Users\Dell\Desktop\demo\project>git clone https://github.com/vaishnavi-9104/git-and-github-assignment.git
Cloning into 'git-and-github-assignment'...
remote: Enumerating objects: 6, done.
remote: Counting objects: 100% (6/6), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 6 (delta 1), reused 6 (delta 1), pack-reused 0
Receiving objects: 100% (6/6), done.
Resolving deltas: 100% (1/1), done.

C:\Users\Dell\Desktop\demo\project>git add script.js

C:\Users\Dell\Desktop\demo\project>git commit -m "Make some changes to script.js"
On branch main
Your branch is up to date with 'origin/main'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        git-and-github-assignment/

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\Dell\Desktop\demo\project>git add <file>
The syntax of the command is incorrect.

C:\Users\Dell\Desktop\demo\project>git add  git-and-github-assignment/
warning: adding embedded git repository: git-and-github-assignment
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint:
hint:   git submodule add <url> git-and-github-assignment
hint:
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint:
hint:   git rm --cached git-and-github-assignment
hint:
hint: See "git help submodule" for more information.
hint: Disable this message with "git config advice.addEmbeddedRepo false"

C:\Users\Dell\Desktop\demo\project>git fetch origin

C:\Users\Dell\Desktop\demo\project>git merge origin/main
Already up to date.

C:\Users\Dell\Desktop\demo\project>git checkout -b feature-update
Switched to a new branch 'feature-update'

C:\Users\Dell\Desktop\demo\project>git add script.js

C:\Users\Dell\Desktop\demo\project>git commit -m "Add updateGreeting function"
[feature-update 474412b] Add updateGreeting function
 2 files changed, 5 insertions(+)
 create mode 160000 git-and-github-assignment

C:\Users\Dell\Desktop\demo\project>git checkout main
warning: unable to rmdir 'git-and-github-assignment': Directory not empty
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

C:\Users\Dell\Desktop\demo\project>git merge feature-update
Updating 2a47060..474412b
Fast-forward
 git-and-github-assignment | 1 +
 script.js                 | 4 ++++
 2 files changed, 5 insertions(+)
 create mode 160000 git-and-github-assignment

C:\Users\Dell\Desktop\demo\project>git add script.js

C:\Users\Dell\Desktop\demo\project>git commit -m "Resolve merge conflicts"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

C:\Users\Dell\Desktop\demo\project>echo.> obsolete.js

C:\Users\Dell\Desktop\demo\project>git rm obsolete.js
fatal: pathspec 'obsolete.js' did not match any files

C:\Users\Dell\Desktop\demo\project>git commit -m "Remove obsolete.js file"
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        obsolete.js

nothing added to commit but untracked files present (use "git add" to track)

C:\Users\Dell\Desktop\demo\project>git reset --hard HEAD~1
warning: unable to rmdir 'git-and-github-assignment': Directory not empty
HEAD is now at 2a47060 Add greetUser function for personalized greeting

C:\Users\Dell\Desktop\demo\project>
