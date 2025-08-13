#merge
==> git merge is used to combine changes from one branch into another.
It takes the commits from a source branch and integrates them into the target branch.

Use of merge:
==> To bring together work from different branches into one branch.
==> Commonly used to combine a other branch into the main branch after development.

Example:
==> If we create a branch called feature-login and completed the login feature, we can merge it into the main branch so that the main project includes the new feature.

Problem scenario: You developed a feature in feature-merge branch and now want it in main.

steps to follow:
git checkout -b merge
echo "Feature for merge" > merge_feature.txt
git add merge_feature.txt
git commit -m "Add merge feature"
git push origin merge

# Merge into main
git checkout main
git merge merge
git push origin main