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
