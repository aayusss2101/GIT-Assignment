# Name: Aayush Mohan Sinha
# Employee ID: TAS124
# GIT-Assignment

Steps Taken:
 
Created an empty repository named GIT-Assignment

Cloned the repository in my local system using the command:
git clone https://github.com/aayusss2101/GIT-Assignment

Created a file in main branch and pushed it to remote, using the following set of commands:
echo "This is a demo file" > demo.text
git add .
git commit -m "Created demo.txt file"
git push origin main

Created branch named Integration and pushed it to remote, using the following commands:
git checkout -b Integration
git push origin Integration

Created branch named HotFix and pushed it to remote, using the following commands:
git checkout -b HotFix
git push origin HotFix

Created two branches, Feature1 and Feature2, from Integration branch, using the following commands:
git checkout -b Feature1 Integration
git checkout -b Feature2 Integration

Switched to Feature2 branch, made some changes and pushed it to remote, using the following commands:
git switch Feature2
echo "This is feature2.txt" > feature2.txt
git add .
git commit -m "Created feature2.txt file in branch Feature2"
git push origin Feature2

Now went to GitHub and created a PR to Integration branch.
After successfully merging deleted the Feature2 branch.

Pulled Integration branch from remote, using the command
git pull origin Integration

Switched to Feature1 branch and made some changes, using the following commands:
git switch Feature1
echo "This is feature1.txt" > feature1.txt
git add .
git commit -m "Created feature1.txt file in branch Feature1"

Rebased Feature1 to Integration, using the following commands:
git rebase Integration Feature1

Switched to Integration branch and pushed the changes to remote, using the command
git push origin Integration

Now went to GitHub and create a PR request from Integration to HotFix branch and main branch and merged the changes after reviewing.

Switched to Feature1 branch, did some changes and pushed it to remote, using the following commands:
git switch Feature1
echo "This is new feature1 file." > newfeature.txt
git add .
git commit -m "Created newfeature1.txt file in Feature1 branch"
git push origin Feature1

Now once again went to GitHub and creatde a PR request from Feature1 to Integration, HotFix and main branch and merged them after review.
Deleted the Feature1 branch.

Switched to HotFix branch, committed some changes and pushed the branch to remote, using the following commands:
git switch HotFix
git pull origin HotFix
echo "This is hotfix file" > hotfix.txt
git add .
git commit -m "Created file hotfix.txt on HotFix Branch"
git push origin HotFix

Finally went to GitHub and created a PR request from HotFix to Integration and main branch and merged the changes after review.
