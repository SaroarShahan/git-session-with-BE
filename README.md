# Learn Enough Git to Be Dangerous

This session focuses on helping developers understand key Git concepts that go beyond the basics but are essential for day-to-day use. It explains differences between important Git operations and introduces advanced commands, emphasizing practical use cases and conflict resolution. The tone is simplified and hands-on, targeting learners who want to become confident with Git in real-world scenarios.

## Topics Covered: 

### Git Pull vs Git Fetch
- **Pull**: Fetches and merges changes from the remote.
- **Fetch**: Only fetches changes; doesn’t merge them.

### Git Merge vs Git Rebase
- **Merge**: Combines branches and creates an extra merge commit.
- **Rebase**: Reapplies commits on top of another branch, creating a cleaner commit history.

### Resolve Rebase Conflicts
- Conflicts can occur during `git rebase`.
- Resolve manually, then use:
  - `git add .` (or specific files)
  - `git rebase --continue`
- If needed:
  - `git rebase --abort` – cancel the rebase
  - `git rebase --skip` – skip the conflicting commit

### Git Cherry-Pick
- Lets you apply a specific commit from one branch to another.
- Useful for selectively moving changes.

### Resolve Cherry-Pick Conflicts
- Handle conflicts during cherry-pick.
- Resolve manually, then use:
  - `git add .` (or specific files)
  - `git cherry-pick --continue`
- If needed:
  - `git cherry-pick --abort` – cancel the rebase

### Git Reset
Moves `HEAD` to a different commit. Used to undo or unstage changes.

- **Hard**: Removes changes from the working directory and the staging area.
- **Soft**: Keeps changes staged; good for amending commits.
- **Mixed** (default): Unstages changes, but keeps them in the working directory.

### Git Stash
Temporarily stores uncommitted changes and reverts your working directory to the last commit.

### Stash Commands:
- `git stash save` – Save current changes.
- `git stash list` – View saved stashes.
- `git stash apply` – Apply a stash without removing it.
- `git stash pop` – Apply and remove the most recent stash.
- `git stash show` – Show what’s inside a stash.
- `git stash drop` – Delete a specific stash.
- `git stash clear` – Remove all stashes.
