#squash merge
==> A squash merge is a way to combine all commits from a branch into one single commit before merging into another branch.
It keeps the commit history clean and concise.

Use of squash merge:
==> To avoid cluttering the main branch with multiple small commits from a feature branch.
==> Ideal for merging experimental or feature branches where commit history is not important to keep individually.

Example:
==> If our feature-login branch has 10 small commits like “fix typo” or “adjust padding,” you can squash them into a single commit and then merge into main with a clean history.

Problem scenario: we made multiple small commits for one feature and want them as one commit in main.

steps to follow:
git checkout -b squash-merge
echo "Part 1" > squash.txt(file name)
git add squash.md
git commit -m "Add part 1"
echo "Part 2" >> squash.txt
git add squash.txt
git commit -m "Add part 2"
git push origin squash-merge