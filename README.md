# Gym-Git-Exercises-Solutions

##Bundle 1

###Exercise 1
```bash
To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.

gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin master
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 588 bytes | 588.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'master' on GitHub by visiting:
remote:      https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions/pull/new/master
remote: 
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
 * [new branch]      master -> master
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git status
On branch master
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git statuis
git: 'statuis' is not a git command. See 'git --help'.

The most similar command is
        status
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git status 
On branch master
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout main
branch 'main' set up to track 'origin/main'.
Switched to a new branch 'main'
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch -m master
fatal: a branch named 'master' already exists
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch -m leader
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push -u origin leader
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'leader' on GitHub by visiting:
remote:      https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions/pull/new/leader
remote: 
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
 * [new branch]      leader -> leader
branch 'leader' set up to track 'origin/leader'.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git status
On branch leader
Your branch is up to date with 'origin/leader'.

nothing to commit, working tree clean
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout master
Switched to branch 'master'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push --set-upstream
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:main

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.

gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push --set-upstream origin master
branch 'master' set up to track 'origin/master'.
Everything up-to-date
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout dev
error: pathspec 'dev' did not match any file(s) known to git
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout -dev
error: unknown switch `e'
usage: git checkout [<options>] <branch>
   or: git checkout [<options>] [<branch>] -- <file>...

    -b <branch>           create and checkout a new branch
    -B <branch>           create/reset and checkout a branch
    -l                    create reflog for new branch
    --guess               second guess 'git checkout <no-such-branch>' (default)
    --overlay             use overlay mode (default)
    -q, --quiet           suppress progress reporting
    --recurse-submodules[=<checkout>]
                          control recursive updating of submodules
    --progress            force progress reporting
    -m, --merge           perform a 3-way merge with the new branch
    --conflict <style>    conflict style (merge, diff3, or zdiff3)
    -d, --detach          detach HEAD at named commit
    -t, --track[=(direct|inherit)]
                          set branch tracking configuration
    -f, --force           force checkout (throw away local modifications)
    --orphan <new-branch>
                          new unparented branch
    --overwrite-ignore    update ignored files (default)
    --ignore-other-worktrees
                          do not check if another worktree is holding the given ref
    -2, --ours            checkout our version for unmerged files
    -3, --theirs          checkout their version for unmerged files
    -p, --patch           select hunks interactively
    --ignore-skip-worktree-bits
                          do not limit pathspecs to sparse entries only
    --pathspec-from-file <file>
                          read pathspec from file
    --pathspec-file-nul   with --pathspec-from-file, pathspec elements are separated with NUL character

gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch -M dev
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout dev
Already on 'dev'
Your branch is up to date with 'origin/master'.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % 
 *  History restored 

gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git log
commit 950ef61987803f08b032e17b5101c2585756f154 (HEAD -> dev, origin/master)
Author: pinsoegustave <ntwalimudasubirag@gmail.com>
Date:   Tue Dec 17 16:41:43 2024 +0200

    new changes

commit 45a19551307f1e8f91cc7a64461cee8e6ce898cc (origin/main, origin/leader, origin/HEAD, leader)
Author: Pinsoe Gustave <108759573+pinsoegustave@users.noreply.github.com>
Date:   Tue Dec 17 16:23:22 2024 +0200

    Initial commit
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch dev
fatal: a branch named 'dev' already exists
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git status
On branch dev
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        style.css

nothing added to commit but untracked files present (use "git add" to track)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add style.css
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit -m "Added two properties"
[dev 1f3631d] Added two properties
 1 file changed, 5 insertions(+)
 create mode 100644 style.css
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin dev 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 352 bytes | 352.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions/pull/new/dev
remote: 
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
 * [new branch]      dev -> dev
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch test
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout dev
Already on 'dev'
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch --delete test
Deleted branch test (was 1f3631d).
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % 
```
###Exercise 2
```bash
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit -m "home.html changes"
[master 0fcc7d4] home.html changes
 1 file changed, 11 deletions(-)
 delete mode 100644 about.html
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash
No local changes to save
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash list
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash     
Saved working directory and index state WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash list
stash@{0}: WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash
Saved working directory and index state WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash list
stash@{0}: WIP on master: 0fcc7d4 home.html changes
stash@{1}: WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git team.html
git: 'team.html' is not a git command. See 'git --help'.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add team.html
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash
Saved working directory and index state WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash list
stash@{0}: WIP on master: 0fcc7d4 home.html changes
stash@{1}: WIP on master: 0fcc7d4 home.html changes
stash@{2}: WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash pop
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

Dropped refs/stash@{0} (1c01f392e5cdc2ecc5595698404e3f9a935d7385)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash pop stash@{1}
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

Dropped stash@{1} (7e0d7826cdb5d8d3d1c2bc7e830b71c1b647f268)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash pop stash@{0}
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
On branch master
Your branch is ahead of 'origin/master' by 2 commits.
  (use "git push" to publish your local commits)

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      about.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   home.html

The stash entry is kept in case you need it again.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit =m "
dquote> >                      
dquote> <
dquote> Setup home and about page"
zsh: m not found
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit -m "
>
<
Setup home and about page"
[master 4c7d481] > < Setup home and about page
 3 files changed, 28 insertions(+), 1 deletion(-)
 create mode 100644 about.html
 create mode 100644 team.html
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
 ! [rejected]        master -> master (fetch first)
error: failed to push some refs to 'https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git pull https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
remote: Enumerating objects: 1, done.
remote: Counting objects: 100% (1/1), done.
remote: Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (1/1), 894 bytes | 298.00 KiB/s, done.
From https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions
 * branch            HEAD       -> FETCH_HEAD
Successfully rebased and updated refs/heads/master.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push                                                                 
Enumerating objects: 12, done.
Counting objects: 100% (12/12), done.
Delta compression using up to 8 threads
Compressing objects: 100% (11/11), done.
Writing objects: 100% (11/11), 1.58 KiB | 1.58 MiB/s, done.
Total 11 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
   4a4feea..f9c75df  master -> master
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash list
stash@{0}: WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash pop          
Auto-merging about.html
CONFLICT (add/add): Merge conflict in about.html
On branch master
Your branch is up to date with 'origin/master'.

Unmerged paths:
  (use "git restore --staged <file>..." to unstage)
  (use "git add <file>..." to mark resolution)
        both added:      about.html

no changes added to commit (use "git add" and/or "git commit -a")
The stash entry is kept in case you need it again.
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git reset --hard
HEAD is now at f9c75df > < Setup home and about page
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % 
```

##Bundle 2

###Exercise 1
```bash
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git branch ft/bundle2
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git log
commit f344efaa85ca83eefcf139850434165a04c6550d (HEAD -> master, origin/master, ft/bundle2)
Author: pinsoegustave <ntwalimudasubirag@gmail.com>
Date:   Wed Dec 18 12:23:16 2024 +0200

    Git: (Bundle 1)Exercise 2

commit f9c75df3e865e7d33f07d063812e1984110be256
Author: pinsoegustave <ntwalimudasubirag@gmail.com>
Date:   Wed Dec 18 12:12:36 2024 +0200

    >
    <
    Setup home and about page

commit 7b35a0564b00c67c967ce2172fb70729a203842a
Author: pinsoegustave <ntwalimudasubirag@gmail.com>
Date:   Wed Dec 18 11:56:21 2024 +0200

    home.html changes

commit 9f375c4303ca65d9b9e444415ec0b4d6db2c1a36
Author: pinsoegustave <ntwalimudasubirag@gmail.com>
Date:   Wed Dec 18 11:53:34 2024 +0200

    Home.html changes

commit 4a4feeac0122a0aed3806795c0a3f74288304474
Merge: 950ef61 8529dd6
Author: Pinsoe Gustave <108759573+pinsoegustave@users.noreply.github.com>
Date:   Wed Dec 18 11:17:39 2024 +0200

    Merge pull request #1 from pinsoegustave/dev
    
    Dev

commit 8529dd6d8bfdb5cba5813d672a061781e777db38
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % 
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
\%                                                                                                                                                                                                                                                                   
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit -m "Git: Services Page"
[master 82b5394] Git: Services Page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin ft/bundle2
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'ft/bundle2' on GitHub by visiting:
remote:      https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions/pull/new/ft/bundle2
remote: 
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
 * [new branch]      ft/bundle2 -> ft/bundle2
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit -m "Edited on home.html" 
[master 64c1417] Edited on home.html
 1 file changed, 1 insertion(+), 1 deletion(-)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin main
error: src refspec main does not match any
error: failed to push some refs to 'https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git'
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin master
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 1.01 KiB | 1.01 MiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
   f344efa..64c1417  master -> master
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git checkout ft/bundle2
M       team.html
Switched to branch 'ft/bundle2'
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash
Saved working directory and index state WIP on ft/bundle2: f344efa Git: (Bundle 1)Exercise 2
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash list
stash@{0}: WIP on ft/bundle2: f344efa Git: (Bundle 1)Exercise 2
stash@{1}: WIP on master: 0fcc7d4 home.html changes
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git stash pop 
On branch ft/bundle2
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   team.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (7ffb916ce80ef2e4cf8d80651ed1343d872e270e)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git add .
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git commit -m "New changes on team page"
[ft/bundle2 224551f] New changes on team page
 1 file changed, 1 insertion(+)
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin ft/bundle
error: src refspec ft/bundle does not match any
error: failed to push some refs to 'https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git'
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % git push origin ft/bundle2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 580 bytes | 580.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/pinsoegustave/Gym-Git-Exercises-Solutions.git
   f344efa..224551f  ft/bundle2 -> ft/bundle2
gymkura@kuras-iMac Gym-Git-Exercises-Solutions % 
```