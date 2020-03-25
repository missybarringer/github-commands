# github-commands
Commonly used github commands
============
Problem: Several links to various sites for different Github commands
Solution: Combine commands into my own repository for future reference

_A list of my commonly used Git commands_

--

### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone [url]` | Create a local copy of a remote repository |

### Basic Snapshotting

| Command | Description |
| ------- | ----------- |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git reset [file-name.txt]` | Unstage a file while retaining the changes in working directory |
| `git add -A` | Add all new and changed files to the staging area |
| `git diff --staged` | diff --staged |
| `git commit -m "[commit message]"` | Commit changes with a descriptive message |
| `git rm -r [file-name.txt]` | Remove a file (or folder) |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch at the current commit |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [new_branch name] [old_branch name]` | Clone a remote branch and switch to it |
| `git checkout -b fix1 origin/fix1` | Create local branch 'fix1' based off origin branch |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge the specified branch's history into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |
| `git stash apply` | Bring your work back |
| `git stash list` | See all of your current stashes |
| `git stash apply stash@{1}` | Apply the second stash (0,1) |
| `git stash pop` | easily apply the top stash on the stack |
| `git stash drop <id>` | deletes that stash for good |
| `git stash clear` | deletes all of the stored stashes |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git push [alias][branch]` | Transmit local branch commits to the remote repository branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git merge[alias]/[branch]` | Merge a remote branch into your current branch to bring it up to date |
| `git fetch [alias]` | fetch down all the branches from that Git remote branch |
| `git remote add origin ssh://git@github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin ssh://git@github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |

### Tracking Path Changes
#### Versioning file removes and path changes
| Command | Description |
| ------- | ----------- |
| `git rm [file]` | Delete the file from project & stage the removal for commit |
| `git mv [existing-path][new-path]` | Change an existing file path & stage the move |
| `git log --stat -M` | Show all commit logs with indication of any paths that moved |

### Rewrite History
#### Rewriting branches, updating commits & clearing history
| Command | Description |
| ------- | ----------- |
| `git rebase [branch]` | Apply any commits of current branch ahead of specified one |
| `git reset --hard[commit]` | Clear staging area, rewrite working tree from specified commit |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git log branchB..branchA` | Show the commits on branchA that are not on branchB |
| `git log --summary` |  |
| `git diff [source branch] [target branch]` | Preview changes before merging |

### Thanks to kumabotz & joshnh for their repositories!
