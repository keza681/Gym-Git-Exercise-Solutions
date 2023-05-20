# Gym-Git-Exercise-Solutions

## Bundle 1

### Exercise 1

```bash
-> lindakezab@LINDAs-MacBook training % git init
Reinitialized existing Git repository in /Users/lindakezab/Desktop/training/.git/
-> lindakezab@LINDAs-MacBook training % git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .DS_Store

nothing added to commit but untracked files present (use "git add" to track)
-> lindakezab@LINDAs-MacBook training % touch Readme.md  
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % git mv Readme.md RE
ADME.md
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % git commit -m "Made changes to the readme file"
[main (root-commit) ad6b9ac] Made changes to the readme file
 2 files changed, 7 insertions(+)
 create mode 100644 .DS_Store
 create mode 100644 README.md
-> lindakezab@LINDAs-MacBook training % git remote add origin https://github.com/keza681/Gym-Git-Exercise-Solutions.git
error: remote origin already exists.
-> lindakezab@LINDAs-MacBook training % git branch -M main
-> lindakezab@LINDAs-MacBook training % git push -u origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 503 bytes | 503.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/keza681/Gym-Git-Exercise-Solutions.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.
-> lindakezab@LINDAs-MacBook training % git branch dev
-> lindakezab@LINDAs-MacBook training % git branch
  dev
* main
-> lindakezab@LINDAs-MacBook training % git checkout dev
Switched to branch 'dev'
-> lindakezab@LINDAs-MacBook training % git checkout -b test
Switched to a new branch 'test'
-> lindakezab@LINDAs-MacBook training % git checkout dev
Switched to branch 'dev'
-> lindakezab@LINDAs-MacBook training % git branch -D test
Deleted branch test (was ad6b9ac).
-> lindakezab@LINDAs-MacBook training % git push -u origin main
branch 'main' set up to track 'origin/main'.
Everything up-to-date
-> lindakezab@LINDAs-MacBook training % git push -u origin dev 
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/keza681/Gym-Git-Exercise-Solutions/pull/new/dev
remote: 
To https://github.com/keza681/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.
-> lindakezab@LINDAs-MacBook training % 
```


#### Exercise 2

```bash
-> lindakezab@LINDAs-MacBook training % touch homme.html
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % 
-> lindakezab@LINDAs-MacBook training % git stash save "home page"
Saved working directory and index state On dev: home page
-> lindakezab@LINDAs-MacBook training % touch aboutt.html
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % git stash save "about page"
Saved working directory and index state On dev: about page
-> lindakezab@LINDAs-MacBook training % touch teamm.html
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % git stash save "team page"
Saved working directory and index state On dev: team page
-> lindakezab@LINDAs-MacBook training % git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   aboutt.html

Dropped stash@{1} (988d7470111216ffe2a81167bac73e3ff12d7894)
-> lindakezab@LINDAs-MacBook training % git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   aboutt.html
        new file:   homme.html

Dropped stash@{1} (380d05683c314496832f1983e869089420ecb32b)
-> lindakezab@LINDAs-MacBook training % git add .
-> lindakezab@LINDAs-MacBook training % git status
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   aboutt.html
        new file:   homme.html

-> lindakezab@LINDAs-MacBook training % git commit -m "Added two files to the directory"
[dev 6f9ebb6] Added two files to the directory
 2 files changed, 24 insertions(+)
 create mode 100644 aboutt.html
 create mode 100644 homme.html
-> lindakezab@LINDAs-MacBook training % git push -u origin dev
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 518 bytes | 518.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/keza681/Gym-Git-Exercise-Solutions.git
   ad6b9ac..6f9ebb6  dev -> dev
branch 'dev' set up to track 'origin/dev'.
-> lindakezab@LINDAs-MacBook training % git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   teamm.html

Dropped stash@{0} (811eea98c0fb7af757cbe372e850bfe9bcef6418)
-> lindakezab@LINDAs-MacBook training % git reset --hard HEAD~1
HEAD is now at ad6b9ac Made changes to the readme file
```
