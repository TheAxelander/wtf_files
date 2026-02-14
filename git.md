# git

| Command | Description |
| --- | --- |
| `git checkout <branch>` | Switch to a branch |
| `git switch <branch>` | Switch to a branch (modern alternative) |
| `git switch -c <branch>` | Create and switch to a new branch |
| `git stash` | Stash current working tree changes |
| `git stash -m "message"` | Stash with a descriptive message |
| `git stash list` | List all stashes |
| `git stash pop` | Apply most recent stash and remove it from the stash list |
| `git stash apply` | Apply most recent stash but keep it in the stash list |
| `git stash pop stash@{n}` | Apply a specific stash and remove it |
| `git commit --amend` | Amend the last commit (message and/or staged changes) |
| `git commit --amend --no-edit` | Amend the last commit without changing the message |
| `git push --force-with-lease` | Force push after amend (safe, checks for remote changes) |
| `git push --force` | Force push after amend (unsafe, overwrites remote) |
| `git push -u origin <branch>` | Set upstream for current branch on first push |
| `git branch --set-upstream-to=origin/<branch>` | Set/update upstream for current branch |
