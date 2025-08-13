rebase
==> git rebase is used to take the changes from one branch and apply them on top of another branch.
It makes commit history linear and clean by avoiding extra merge commits.

Use of git rebase
==> Update the branch with the latest changes from another branch without creating a merge commit.
==> Makes it look like you started work from the most recent version of that branch.

Example:
==> We are working on a feature branch while the main branch has received new commits.
==>Instead of merging,we can run:
git checkout feature
git rebase main