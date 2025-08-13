#staging
==> Staging is the process of preparing changes before committing them to the repository.
It’s like putting files into a waiting area so Git knows exactly which changes you want to commit.

Use of staging:
==> Allows us to control which changes go into next commit.
==> we can stage only specific files or even specific parts of a file.

Example:
==> If we edit 5 files but only 2 are ready to commit, we can stage those 2 files and leave the rest unstaged until they’re ready.

Problem scenario: You have two files but want to commit only one for now. Adding to staging area which are ready to commit and done with the changes.

steps to follow:
git checkout -b staging
echo "Bug fix line" > bugfix.txt
echo "Feature added line" > feature.txt
git add feature.txt
git commit -m "Commit only feature file"
git push origin staging