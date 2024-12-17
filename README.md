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
