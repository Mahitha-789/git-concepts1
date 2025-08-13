#push
==> git push is used to upload local commits to a remote repository.
It sends branch changes to the remote branch so others can access your work.

Use of git push:
==> To Share latest work with your team.
==> Save local commits in the remote repository for backup and collaboration.

Example:
==> After making changes in local project and commit them, we can use git push to send those commits to GitHub so teammates can pull the latest version.

Problem scenario: You made a new file feature.txt locally and need to share it on GitHub.

steps to follow:
git checkout -b push
echo "My new feature" > feature.txt
git add feature.txt
git commit -m "Add new feature file"
git push origin push