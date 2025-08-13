#pull
==> git pull is used to fetch and merge changes from a remote repository into your current local branch.
It updates your local copy with the latest changes from the remote branch.

Use of git pull:
==> Keep your local branch up to date with the remote branch.
==> Get the latest commits made by other team members.

Example:
==> If you are already working on a project locally and your teammates push new changes to GitHub, you can run git pull to bring those changes into your local project.

Problem scenario: Teammate updated team.txt on GitHub. Your local repo doesn’t have it yet.

steps to follow:
#teammate change
git checkout -b pull
echo "Initial version" > team.txt
git add team.txt
git commit -m "Initial team file"
git push origin pull

#getting locally:
git pull origin pull