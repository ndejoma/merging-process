# Merging process in Git

## A Fast forward merge
 - A fast-forward merge is possible when there are no further commit created in the **receiving branch** after the branch being merged was created. eg a **feature branch**

 - It just move the **main** branch pointer to the last commit in the **feature_branch**

 ### Fast-forward Merging process 
 1. Create a new branch called **feature-1** from the **main** branch.
 2. Make changes in the new branch and commit them.
 3. Checkout the **main** branch, in this case which will be the receiving branch.
 4. Merge the feature branch into the current receiving branch

 ```shell
 git checkout -b feature-1

 git commit -a -m "changes in  the feature 1 branch"

 git checkout main

 git merge feature-1