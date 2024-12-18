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