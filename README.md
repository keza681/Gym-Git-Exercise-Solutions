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


### Exercise 2

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



## Bundle 2

### Exercise 1

```bash
/Users/lindakezab/.zshrc:9: command not found: rbenv
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout -b ft/bundle
-2
Switched to a new branch 'ft/bundle-2'
-> lindakezab@LINDAs-MacBook Git-Practice % touch services.html
-> lindakezab@LINDAs-MacBook Git-Practice % git add .
-> lindakezab@LINDAs-MacBook Git-Practice % git add .               
-> lindakezab@LINDAs-MacBook Git-Practice % git commit -m "Made some changes to services. html file"
[ft/bundle-2 f743302] Made some changes to services. html file
 1 file changed, 12 insertions(+)
 create mode 100644 services.html
-> lindakezab@LINDAs-MacBook Git-Practice % git push -u origin ft/bun
dle-2
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 267 bytes | 133.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/keza681/Git-Practice/pull/new/ft/bundle-2
remote: 
To https://github.com/keza681/Git-Practice.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
-> lindakezab@LINDAs-MacBook Git-Practice % 
```


### Exercise 2

```bash
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout -b ft-service-redesign
Switched to a new branch 'ft-service-redesign'
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit -
m "Made some changes to the service page"    
[ft-service-redesign ce044a6] Made some changes to the service page
 1 file changed, 1 insertion(+), 1 deletion(-)
-> lindakezab@LINDAs-MacBook Git-Practice % git push -u origin ft-ser
vice-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 349 bytes | 349.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft-service-redesign' on GitHub by visiting:
remote:      https://github.com/keza681/Git-Practice/pull/new/ft-service-redesign
remote: 
To https://github.com/keza681/Git-Practice.git
 * [new branch]      ft-service-redesign -> ft-service-redesign
branch 'ft-service-redesign' set up to track 'origin/ft-service-redesign'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit -
m "Add new changes to the service page"
[main 7cfcd42] Add new changes to the service page
 1 file changed, 1 insertion(+), 1 deletion(-)
-> lindakezab@LINDAs-MacBook Git-Practice % git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 347 bytes | 347.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/keza681/Git-Practice.git
   1fb136c..7cfcd42  main -> main
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout ft-service-r
edesign
Switched to branch 'ft-service-redesign'
Your branch is up to date with 'origin/ft-service-redesign'.
-> lindakezab@LINDAs-MacBook Git-Practice % git diff main..ft-service
-redesign
diff --git a/services.html b/services.html
index 7428d29..e8da765 100644
--- a/services.html
index 7428d29..e8da765 100644
--- a/services.html
index 7428d29..e8da765 100644
--- a/services.html
+++ b/services.html
@@ -7,6 +7,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1>Hello ojemba x The Gym</h1>
+    <h1>hello Ojemba x The gym</h1>
 </body>
 </html>
\ No newline at end of file
(END)
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit -m "fix conflict"
[ft-service-redesign e0af171] fix conflict
-> lindakezab@LINDAs-MacBook Git-Practice % git push 
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 218 bytes | 218.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/keza681/Git-Practice.git
   ce044a6..e0af171  ft-service-redesign -> ft-service-redesign
```

## Bundle 3


### Exercise 1

```bash
Book Git-Practice % git push -u origin ft/tea
m-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 250 bytes | 250.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/keza681/Git-Practice/pull/new/ft/team-page
remote: 
To https://github.com/keza681/Git-Practice.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout -b ft/contac
t-page
Switched to a new branch 'ft/contact-page'
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout ft/team-page

Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
-> lindakezab@LINDAs-MacBook Git-Practice % git log
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmai
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf5
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf599
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +02
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 10:53:02 2023 +0200
:
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout 
ft/contact-page
Switched to branch 'ft/contact-page'
-> lindakezab@LINDAs-MacBook Git-Practice % git
-> lindakezab@LINDAs-MacBook Git-Practice % git cherry-pick 2223b32e0f51961fd6ce97dad06e3f3c88b3483b
[ft/contact-page 63df400] Add new file for team page
 Date: Mon May 22 11:08:48 2023 +0200
 1 file changed, 12 insertions(+)
 create mode 100644 team.html
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && 
git commit -m "Update contact page"
[ft/contact-page 7bc1bb8] Update contact page
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 contact.html
-> lindakezab@LINDAs-MacBook Git-Practice % git push -u o
rigin ft/contact-page
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 520 bytes | 260.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/keza681/Git-Practice/pull/new/ft/contact-page
remote: 
To https://github.com/keza681/Git-Practice.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout 
-b ft/faq-page
Switched to a new branch 'ft/faq-page'
-> lindakezab@LINDAs-MacBook Git-Practice % touch faq.htm
l
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && 
git commit -m "Add new file faq.html page"
[ft/faq-page 465026b] Add new file faq.html page
 1 file changed, 12 insertions(+)
 create mode 100644 faq.html
-> lindakezab@LINDAs-MacBook Git-Practice % git push -u o
rigin ft/faq-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 245 bytes | 245.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/keza681/Git-Practice/pull/new/ft/faq-page
remote: 
To https://github.com/keza681/Git-Practice.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout 
ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.
-> lindakezab@LINDAs-MacBook Git-Practice % git log
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +02
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author:
commit 2223b32e0f51961fd6ce97dad06e3f3c88b3483b (HEAD -> ft/team-page, origin/ft/team-page)
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 11:08:48 2023 +0200

    Add new file for team page

commit e0af171f9e57a3deea1ea6cbbf59981c2ee6ed7d (origin/ft-service-redesign, ft-service-redesign)
Merge: ce044a6 7cfcd42
Author: Martine Linda <lindakeza19@gmail.com>
Date:   Mon May 22 10:53:02 2023 +0200
:
nce   e
diting star  t
ed
See ":help   W
11" for mor  e
 info.
[O]K, (L)oa  d
-- More
 File, Load File (a)nd Options: 
 -> lindakezab@LINDAs-MacBook Git-Practice % git push 
Everything up-to-date
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && 
git commit -m "Reverted last commit"
[ft/team-page 8ad0db1] Reverted last commit
 1 file changed, 12 deletions(-)
 delete mode 100644 team.html
-> lindakezab@LINDAs-MacBook Git-Practice % git push 
Enumerating objects: 3, done.
Counting objects:  33% (1/3Counting objects:  66% (2/3Counting objects: 100% (3/3Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects:  50% (Compressing objects: 100% (Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 234 bytes | 234.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas:  remote: Resolving deltas: 1remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/keza681/Git-Practice.git
   2223b32..8ad0db1  ft/team-page -> ft/team-page
-> lindakezab@LINDAs-MacBook Git-Practice % 
```

### Exercise 2
```bash
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout ft/faq-page
Switched to branch 'ft/faq-page'
Your branch is up to date with 'origin/ft/faq-page'.
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout -b ft/home-p
age-redesign
Switched to a new branch 'ft/home-page-redesign'
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit -
m "Update the main branch"
[main d49b2b6] Update the main branch
 1 file changed, 1 insertion(+), 1 deletion(-)
-> lindakezab@LINDAs-MacBook Git-Practice % git checkout ft/home-page
-redesign
Switched to branch 'ft/home-page-redesign'
-> lindakezab@LINDAs-MacBook Git-Practice % git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit "
Rebased the main branch to this branch and add changes to the home page"
error: pathspec 'Rebased the main branch to this branch and add changes to the home page' did not match any file(s) known to git
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit m "Rebased the main branch to this branch and add changes to the home page"
error: pathspec 'm' did not match any file(s) known to git
error: pathspec 'Rebased the main branch to this branch and add changes to the home page' did not match any file(s) known to git
-> lindakezab@LINDAs-MacBook Git-Practice % git add . && git commit -m "Rebased the main branch to this branch and add changes to the home page"
[ft/home-page-redesign e256932] Rebased the main branch to this branch and add changes to the home page
 1 file changed, 1 insertion(+), 1 deletion(-)
-> lindakezab@LINDAs-MacBook Git-Practice % git push -u origin ft/hom
e-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (13/13), 1.34 KiB | 684.00 KiB/s, done.
Total 13 (delta 6), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (6/6), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/keza681/Git-Practice/pull/new/ft/home-page-redesign
remote: 
To https://github.com/keza681/Git-Practice.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
-> lindakezab@LINDAs-MacBook Git-Practice % 
```
