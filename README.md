#### Create and switch to a new branch named `"learnDevOps"`
`git checkout -b learnDevOps`
#### Explanation: This command creates a new branch named "learnDevOps" and switches to it. You are now ready to make changes on this branch without affecting the main branch.

#### Make and commit your changes
`git add .`
`git commit -m "Add initial DevOps scripts"`
#### Explanation: Use git add . to stage all changes and git commit -m to commit your changes with a meaningful message describing what you've done.

#### Fetch the latest changes from the remote main branch
`git fetch origin main`
#### Explanation: git fetch downloads objects and refs from another repository without making any changes to your local repository. It's a good practice to fetch changes from the remote before rebasing.

#### Rebase your branch onto the latest changes from main
`git rebase origin/main`
#### Explanation: A rebase applies your changes on top of the latest changes from another branch, in this case, the main branch. This keeps your branch up to date with the latest developments while maintaining a clean commit history.

#### Check who last modified each line of a file
`git blame filename.ext`
#### Explanation: The git blame command shows you who last modified each line of a file, along with the commit that introduced the change. It's useful for tracking down the origin of specific changes or understanding code authorship.

#### Push your changes to the remote repository
`git push origin learnDevOps`
#### Explanation: Use git push to send your local commits to the remote repository. This step ensures your changes are accessible to other collaborators.

#### Merge your changes into the main branch (optional)
`git checkout main`
`git merge learnDevOps`
#### Explanation: If you've finished working on your branch and want to incorporate your changes into the main branch, use git merge to combine the two branches.

#### Delete the local branch after merging (optional)
`git branch -d learnDevOps`
#### Explanation: If you've merged your changes and no longer need the learnDevOps branch, you can use git branch -d to delete it from your local repository.

#### Delete the remote branch after merging (optional)
`git push origin --delete learnDevOps`
#### Explanation: To remove the learnDevOps branch from the remote repository after merging, use git push with the --delete flag.

#### Create and switch to a new branch named "learnDevOps"
git checkout -b learnDevOps
#### Explanation: This command creates a new branch named "learnDevOps" and switches to it. You are now ready to make changes on this branch without affecting the main branch.

#### Make and commit your changes
`git add .`
`git commit -m "Add initial DevOps scripts"`
#### Explanation: Use git add . to stage all changes and git commit -m to commit your changes with a meaningful message describing what you've done.

#### Fetch the latest changes from the remote main branch
`git fetch origin main`
#### Explanation: git fetch downloads objects and refs from another repository without making any changes to your local repository. It's a good practice to fetch changes from the remote before rebasing.

#### Rebase your branch onto the latest changes from main
git rebase origin/main
#### Explanation: The git rebase command applies your commits on top of the latest changes from the specified branch (in this case, origin/main). This keeps your branch's commit history linear and avoids unnecessary merge commits.

#### Push your changes to the remote repository
`git push origin learnDevOps`
#### Explanation: Use git push to send your local commits to the remote repository. This step ensures your changes are accessible to other collaborators.

#### Delete the local branch after merging (optional)
`git branch -d learnDevOps`
#### Explanation: If you've merged your changes and no longer need the learnDevOps branch, you can use git branch -d to delete it from your local repository.

#### Delete the remote branch after merging (optional)
`git push origin --delete learnDevOps`
#### Explanation: To remove the learnDevOps branch from the remote repository after merging, use git push with the --delete flag.

#### Remember that while rebasing can provide a cleaner commit history, it can also rewrite commit history and may introduce conflicts that need to be resolved. Use rebasing carefully and consider its implications, especially when collaborating with others on a shared repository.
----------------------------------------

