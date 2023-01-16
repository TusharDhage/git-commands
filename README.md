# git-commands
 git config --global user.name “Tushar Dhage”</br>
 git config --global user.email “tushar.dhage95@gmail.com”</br>
 git pull origin master —</br>
 git status</br>
 git remote -v</br>
 git rebase -i master - Suppose you have pulled master and before you commit your code someone else committed the code then you have to rebase your master in order to commit your code.</br>
 git pull</br>
 git config pull.rebase false —>If the system asks you to run this command</br>
 git pull origin master —> this needs to be run in working branch if working branch is not in sync with master branch.</br>
 a-> git stash - This will save the data into your local.</br>
 b-> git stash pop —> checkout in newly created branch and run this command which Will apply all the changes from your local to your branch. Now, you can commit your code. This will apply the changes and also delete the saved data from temporary memory</br>
 b-> git stash apply —>this will apply the changes into the branch and also keep the data in temporary memory</br>
 git status</br>
 git commit -am “Test Fixes” —> Commit the code and in double quotes will write the comments regarding the code</br>
 git push -u origin CQA-627-Regression-issue-fixes. —> After Commit Push the code into the branch. CQA-627 is the Jira tickets ID and append with the the Jira title. Remove spaces with “-” or “_”either way works.</br>
 git checkout master —> To keep your branch unto date after push</br>
 git status —> To know the status if all codes are committed or anything is still pending</br>
 git branch —> This will. Show you the current branch in which you are on.</br>
 git checkout “Branchname” —> This will point to the branch you want to.</br>
 git checkout -b “JiraiD-title” —> This will create a new branch</br>
 git branch -D “branchname” —> this will delete the branch from your local</br>
 git branch -d “branchname” —> this will delete the branch from your local and from UI GitHub as well which we will delete manually</br>
———————————————————————————————></br>
**If git shows conflicts then force push needs to be done.**</br>
**Below steps to be followed.**</br>
Navigate to master -> git pull till you get message “Already upto date”.</br>
Then navigate back to your branch in which conflict is present</br>
git rebase -i master and enter then type “:wq+enter” to exit editor.</br>
git push —force origin “branch name”- this will force push the changes.</br>
This will resolve the conflicts.</br>
