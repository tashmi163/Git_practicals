# Git_practicals
#connect github with vscode

git version 2.43.0.windows.1
PS Z:\GIT> git onfig --global user.name "tashmi163"
git: 'onfig' is not a git command. See 'git --help'.

The most similar command is
        config
PS Z:\GIT> git config --global user.name "tashmi163"
PS Z:\GIT> git config --global user.email "tesharaperera@gmail.com"
PS Z:\GIT> git init
Initial commit

  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)
PS Z:\GIT> git add index.html
PS Z:\GIT> git branch -M main  
PS Z:\GIT> git remote add origin https://github.com/tashmi163/Git_practicals.git
PS Z:\GIT> git push -u origin main
error: failed to push some refs to 'https://github.com/tashmi163/Git_practicals.git'
PS Z:\GIT> git push 
fatal: The current branch main has no upstream branch.

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

PS Z:\GIT> git commit -m "Initial commit"
[main (root-commit) 58df5d6] Initial commit
 1 file changed, 11 insertions(+)
PS Z:\GIT> git push -u origin main
info: please complete authentication in your browser...
To https://github.com/tashmi163/Git_practicals.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/tashmi163/Git_practicals.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
PS Z:\GIT> git pull origin main --rebase
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 862 bytes | 6.00 KiB/s, done.
From https://github.com/tashmi163/Git_practicals
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
Successfully rebased and updated refs/heads/main.
PS Z:\GIT> git push -u origin main       
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 430 bytes | 39.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/tashmi163/Git_practicals.git
   db457db..55fbb7d  main -> main
branch 'main' set up to track 'origin/main'.
PS Z:\GIT> 
