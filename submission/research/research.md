Git Squash

Git squash combines many commits into one commit.

Example:
You made 3 small commits:

Add login button

Fix login button

Change login button text

You can squash them into one commit:
Add login feature

Git Rebase

Git rebase moves your commits on top of another branch.

It can make the Git history cleaner.

Example:
You are working on feature/login.
The main branch has new commits.

You can update your branch with:
git rebase main

Git Merge

Git merge combines two branches together.

It may create a merge commit.

Example:
You finished the login feature on feature/login.

Go to main:
git switch main

Then merge:
git merge feature/login

Git Revert

Git revert cancels the changes of an old commit by creating a new commit.

It is safe to use in shared repositories.

Example:
A commit caused a problem.

Use:
git revert abc123

Git creates a new commit that cancels the old changes.

Git Cherry-Pick

Git cherry-pick takes one specific commit from another branch and adds it to your current branch.

Example:
Ahmed made an important fix in another branch.

The commit ID is abc123.

Use:
git cherry-pick abc123

Git Clean

Git clean removes untracked files from the project.

Use it carefully because deleted files can be lost.

Example:
You have test files that Git does not track.

First check:
git clean -n

Then remove:
git clean -f

Git Grep

Git grep searches for text inside project files.

Example:
You want to find the word password.

Use:
git grep "password"

Git Blame

Git blame shows who changed each line in a file and which commit made the change.

Example:
You want to know who changed a line in Program.cs.

Use:
git blame Program.cs

Git Bisect

Git bisect helps find the commit that caused a bug.

It checks commits step by step.

Example:
The app worked before, but now it has a bug.

Start:
git bisect start

Mark the current commit as bad:
git bisect bad

Mark an old working commit as good:
git bisect good abc123

Git helps you find the bad commit.

Git Shortlog

Git shortlog shows a short summary of commits.

It can group commits by author.

Example:
You want to see commits grouped by developer.

Use:
git shortlog

Git Prune

Git prune removes old Git objects that are no longer needed.

Example:
Git has old unused objects.

Use:
git prune

This command is usually used automatically by Git.

Git Worktree

Git worktree lets you have more than one working directory for the same repository.

This helps you work on two branches at the same time.

Example:
You are working on feature/login,
but you also need to fix a bug on main.

Use:
git worktree add ../main-fix main

Now you can open another folder for main.

Git Verify-Commit

Git verify-commit checks if a commit has a valid GPG signature.

Example:
You want to check if commit abc123 is signed.

Use:
git verify-commit abc123

Git Filter-Repo

Git filter-repo changes or cleans Git history.

Example:
You accidentally committed a secret file called .env.

You can remove it from Git history using git filter-repo.

Example command:
git filter-repo --path .env --invert-paths

Git Help

Git help shows information about Git commands.

Example:
You do not remember how merge works.

Use:
git help merge

Git will show help for the merge command.