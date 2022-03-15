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
```

## A three-way merge process
===============================
 - Happens when there are new commit in the receiving since the current branch was created.

 - A new merge commit is created which is the parent of the last two commits being merge

### Three way merging process

During a three way merge-process, if the same file was edited in both branches, a merge conflict will happen. To resolve the conflict manually, you can use an editor/; lke nano and VScode.
- You can decide:

  1. Keep both changes you made
  2. Accept changes from the incoming  branch in this case the **merge-conflict** branch
  3. You can also decide to keep the changes in the receiving branch
 - A merge conflict may happen during three-way merge process, when you make changes to to the same file before the merge commit is created
 - Git will ask you to resolve all the conflict before it proceeds with the merge of the two branches
 
 


