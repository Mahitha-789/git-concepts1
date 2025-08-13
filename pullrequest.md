pull request
==> A pull request is a request to merge changes from one branch into another branch in a remote repository in GitHub.
It is mainly used for code review before merging.

Use of pull request
==> Share your code changes with the team for review.
==> Discuss improvements, find mistakes, and approve before merging.

Example:
==> You created a new branch feature-login, made changes, and pushed it to GitHub.
Then you open a pull request to merge feature-login into main.
Your teammates will review and approve before it gets merged.

Problem scenario: You finished work in pullrequest-demo and want it reviewed before merging to main.

steps to follow:
git checkout -b pullrequest
git add pullrequest.md
git commit -m "Add pull request demo file"
git push origin pullrequest