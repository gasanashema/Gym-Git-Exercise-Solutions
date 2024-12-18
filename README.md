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


```
