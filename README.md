# Gym-Git-Exercise-Solutions

## Bundle 1
### Exercise 1


```bash
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git init
hint: Using 'master' as the name for the initial branch. This default branch name
hint: is subject to change. To configure the initial branch name to use in all
hint: of your new repositories, which will suppress this warning, call:
hint: 
hint:   git config --global init.defaultBranch <name>
hint: 
hint: Names commonly chosen instead of 'master' are 'main', 'trunk' and
hint: 'development'. The just-created branch can be renamed via this command:
hint: 
hint:   git branch -m <name>
Initialized empty Git repository in /home/shema/New Volume data/The Gym/Gym-Git-Exercise-Solutions/.git/

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git branch -m main

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        break camel casing.js

nothing added to commit but untracked files present (use "git add" to track)

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m 'initial commit'
[main (root-commit) c5c0996] initial commit
 1 file changed, 11 insertions(+)
 create mode 100644 break camel casing.js

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git remote add origin git@github.com:gasanashema/Gym-Git-Exercise-Solutions.git

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git config pull.rebase true

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git pull origin main
From github.com:gasanashema/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
warning: skipped previously applied commit c5c0996
hint: use --reapply-cherry-picks to include skipped commits
hint: Disable this message with "git config advice.skippedCherryPicks false"
Successfully rebased and updated refs/heads/main.

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin main
Everything up-to-date

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b dev
Switched to a new branch 'dev'

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b test
Switched to a new branch 'test'

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout dev
Switched to branch 'dev'

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git branch -d test
Deleted branch test (was 345053d).
```

### Exercise 2

```bash

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git stash -u
Saved working directory and index state WIP on dev: 02ce0c5 Update README.md

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git stash -u
Saved working directory and index state WIP on dev: 02ce0c5 Update README.md

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git stash -u
Saved working directory and index state WIP on dev: 02ce0c5 Update README.md

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{1}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{1} (463b460d46acdcb7a3e93a33264f8f9af60e958b)

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{1}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{1} (ed3a09cfba98cddcce17ba3e3cddafb02521d74c)

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git add . 

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git commit -m 'Using stash to temporarly save files'
[dev 0a9b3d7] Using stash to temporarly save files
 2 files changed, 78 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git push origin dev
Enter passphrase for key '/Users/gymgukunda/.ssh/id_ed25519': 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.33 KiB | 1.33 MiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
   7fa7e55..0a9b3d7  dev -> dev

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git stash pop stash@{0}
Already up to date.
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)
Dropped stash@{0} (fa762631a277c1cab058f55cca02668dd75ca4c9)

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git reset

```

## Bundle 2
### Exercise 1

```bash
gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git branch ft/bundle-2

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git branch
* dev
  ft/bundle-2
  main

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git checkout ft/bundle-2
Switched to branch 'ft/bundle-2'

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git add .

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git commit -m 'added services.html'
[ft/bundle-2 3f11542] added services.html
 1 file changed, 39 insertions(+)
 create mode 100644 services.html

gymgukunda@Gukundas-iMac Gym-Git-Exercise-Solutions % git push origin ft/bundle-2
Enter passphrase for key '/Users/gymgukunda/.ssh/id_ed25519': 
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 244 bytes | 244.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2

```

### Exercise 2

```bash
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git branch
  dev
  ft/service-redesign
* main
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git diff main
diff --git a/services.html b/services.html
index 700096b..b50c01d 100644
--- a/services.html
+++ b/services.html
@@ -25,11 +25,7 @@
       <button type="button" class="btn btn-dark my-4" id="button">Dark</button>
 
 
-      <article id="content">
-        <p>Brownie lollipop <span>carrot cake</span> gummies lemon drops sweet roll dessert tiramisu. Pudding muffin <
span>cotton candy</span> croissant fruitcake tootsie roll. Jelly jujubes brownie. Marshmallow jujubes topping sugar plu
m jelly jujubes chocolate.</p>
-        
-        <p>Tart bonbon soufflé gummi bears. Donut marshmallow <span>gingerbread cupcake</span> macaroon jujubes muffin. Soufflé candy caramels tootsie roll powder sweet roll brownie <span>apple pie</span> gummies. Fruitcake danish chocolate tootsie roll macaroon.</p>
-      </article>
+      
     </div>

     shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git merge main
Already up to date.

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m "conflicts resolved"
[ft/service-redesign 0ddb8c0] conflicts resolved
 1 file changed, 33 insertions(+), 1 deletion(-)

 shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/service-redesign
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 877 bytes | 877.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
   dc53444..0ddb8c0  ft/service-redesign -> ft/service-redesign

```

## Bundle 3
### Exercise 1

```bash
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m 'added teams.html page'
[ft/team-page 03fe976] added teams.html page
 2 files changed, 40 insertions(+), 39 deletions(-)
 delete mode 100644 team.html
 create mode 100644 teams.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1011 bytes | 1011.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/team-page
Switched to branch 'ft/team-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git log
commit 03fe9761669780a91d342305ebadbea01d10135f (HEAD -> ft/team-page, origin/ft/team-page)
Author: Shema <shemaphilbert8@gmail.com>
Date:   Wed Dec 18 14:44:06 2024 +0200

    added teams.html page

commit 8b9466385c10120635fe99b1a6d481097de4bdc2 (main, ft/service-redesign, ft/contact-page)
Author: Shema <shemaphilbert8@gmail.com>
...skipping...

                   SUMMARY OF LESS COMMANDS

      Commands marked with * may be preceded by a number, N.
      Notes in parentheses indicate the behavior if N is given.
      A key preceded by a caret indicates the Ctrl key; thus ^K is ctrl-K.

  h  H                 Display this help.
  q  :q  Q  :Q  ZZ     Exit.
HELP -- Press RETURN for more, or q when done...skipping...
commit 03fe9761669780a91d342305ebadbea01d10135f (HEAD -> ft/team-page, origin/ft/team-page)
Author: Shema <shemaphilbert8@gmail.com>
Date:   Wed Dec 18 14:44:06 2024 +0200

    added teams.html page

commit 8b9466385c10120635fe99b1a6d481097de4bdc2 (main, ft/service-redesign, ft/contact-page)
Author: Shema <shemaphilbert8@gmail.com>

[1]+  Stopped                 git log
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git cherry-pick 03fe9761669780a91d342305ebadbea01d10135f 
On branch ft/team-page
You are currently cherry-picking commit 03fe976.
  (all conflicts fixed: run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

nothing to commit, working tree clean
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git branch
  dev
  ft/contact-page
  ft/service-redesign
* ft/team-page
  main
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
warning: cancelling a cherry picking in progress
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/team-page
Switched to branch 'ft/team-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add contact.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m 'changed contact page'
[ft/team-page a418f11] changed contact page
 1 file changed, 35 insertions(+)
 create mode 100644 contact.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/team-page
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 239 bytes | 239.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
   03fe976..a418f11  ft/team-page -> ft/team-page
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/contact-page
ssh: connect to host ssh.github.com port 443: Connection timed out
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/contact-page
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout rf/contact-page
error: pathspec 'rf/contact-page' did not match any file(s) known to git
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git branch
  dev
  ft/contact-page
  ft/service-redesign
* ft/team-page
  main
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/contact-page
Switched to branch 'ft/contact-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add faq.html 
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m 'added faq page'
[ft/faq-page 9e1f7cc] added faq page
 1 file changed, 36 insertions(+)
 create mode 100644 faq.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/faq-page
ssh: connect to host ssh.github.com port 443: Connection timed out
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.20 KiB | 1.20 MiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote: 
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/team-page
Switched to branch 'ft/team-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git log
commit a418f11a5899e51fedb95eccb895528b6a08f19a (HEAD -> ft/team-page, origin/ft/team-page)
Author: Shema <shemaphilbert8@gmail.com>
Date:   Wed Dec 18 15:10:00 2024 +0200

    changed contact page

commit 03fe9761669780a91d342305ebadbea01d10135f
Author: Shema <shemaphilbert8@gmail.com>

[2]+  Stopped                 git log
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git revert a418f11a5899e51fedb95eccb895528b6a08f19a
[ft/team-page 873e7ee] Revert "changed contact page"
 1 file changed, 35 deletions(-)
 delete mode 100644 contact.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m 'revert contact page commit'
On branch ft/team-page
nothing to commit, working tree clean
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/contact-page
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 ! [rejected]        ft/contact-page -> ft/contact-page (non-fast-forward)
error: failed to push some refs to 'github.com:gasanashema/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because a pushed branch tip is behind its remote
hint: counterpart. If you want to integrate the remote changes, use 'git pull'
hint: before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ 



```


### Exercise 2

```bash

  shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git branch
  dev
  ft/contact-page
  ft/faq-page
  ft/service-redesign
* ft/team-page
  main
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/faq-page
Switched to branch 'ft/faq-page'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m 'changed home.html'
[main af8116e] changed home.html
 1 file changed, 2 insertions(+)
 shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push -f origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 323 bytes | 323.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 + ed5bc85...af8116e main -> main (forced update)
 
 shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git rebase main
Successfully rebased and updated refs/heads/ft/home-page-redesign.
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add home.html 
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m ' modified home on home-page-redesign branch'
[ft/home-page-redesign 8979ead]  modified home on home-page-redesign branch
 1 file changed, 2 insertions(+), 1 deletion(-)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/home-page-redesign
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.55 KiB | 1.55 MiB/s, done.
Total 6 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ 

 ```

## Bundle 4
### Exercise 1

```bash
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout main
Switched to branch 'main'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git remote add git-copy git@github.com:gasanashema/Gym-git-copy.git
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git remote -v
git-copy        git@github.com:gasanashema/Gym-git-copy.git (fetch)
git-copy        git@github.com:gasanashema/Gym-git-copy.git (push)
origin  git@github.com:gasanashema/Gym-Git-Exercise-Solutions.git (fetch)
origin  git@github.com:gasanashema/Gym-Git-Exercise-Solutions.git (push)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ echo "<p>Updated Home Page</p>" >> index.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ echo "<p>Updated Home Page</p>" >> home.html
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m "Updated the home page content"
[main fd3a016] Updated the home page content
 1 file changed, 1 insertion(+), 1 deletion(-)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin main
ssh: connect to host ssh.github.com port 443: Connection timed out
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin main
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 321 bytes | 321.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
   af8116e..fd3a016  main -> main
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push git-copy main
Enumerating objects: 41, done.
Counting objects: 100% (41/41), done.
Delta compression using up to 4 threads
Compressing objects: 100% (39/39), done.
Writing objects: 100% (41/41), 9.72 KiB | 1.39 MiB/s, done.
Total 41 (delta 17), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (17/17), done.
To github.com:gasanashema/Gym-git-copy.git
 * [new branch]      main -> main

```
## Bundle 4
### Exercise 2

```bash

shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m "added changes on this branch"
[ft/footer 58a4ff5] added changes on this branch
 1 file changed, 3 insertions(+), 2 deletions(-)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git add .
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m "added another changes on this branch and I am going to make the second commit"
[ft/footer 8457cea] added another changes on this branch and I am going to make the second commit
 1 file changed, 1 insertion(+), 4 deletions(-)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/footer
Enumerating objects: 11, done.
Counting objects: 100% (11/11), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (9/9), 905 bytes | 905.00 KiB/s, done.
Total 9 (delta 6), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (6/6), completed with 2 local objects.
remote: 
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ 
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout main
M       README.md
Switched to branch 'main'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git merge --squash ft/footer
Updating 8ee7d77..30167bb
Fast-forward
Squash commit -- not updating HEAD
 home.html | 10 ++++------
 1 file changed, 4 insertions(+), 6 deletions(-)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git commit -m "Footer changes squashing"
[ft/squashing b07bda5] Footer changes squashing
 2 files changed, 36 insertions(+), 6 deletions(-)
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ git push origin ft/squashing
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 744 bytes | 744.00 KiB/s, done.
Total 4 (delta 3), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
remote: 
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/gasanashema/Gym-Git-Exercise-Solutions/pull/new/ft/squashing
remote: 
To github.com:gasanashema/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/squashing -> ft/squashing
shema@shema:~/New Volume data/The Gym/Gym-Git-Exercise-Solutions$ 


```