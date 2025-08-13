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

Problem scenario: Your branch is behind main, but you want a clean history before merging.

steps to follow:
git checkout -b rebase
git add rebase.md
git commit -m "Add rebase work"

# Simulate main branch getting updated:
git checkout main
git add main_update.txt(file.name)
git commit -m "Update main branch"
git push origin main

# Rebase your branch onto updated main
git checkout rebase
git rebase main
git push origin rebase --force