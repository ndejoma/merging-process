## Three way merging process
1. Create a new branch called **feature-2**
   ```shell
   git branch feature1
   ```

2. Switch to that branch or just checkout the branch
   ```shell
   git switch feature-2 || git checkout feature-2
   ```
3. Make change and commit them.
   ```shell
   git commit -a -m "Feature 2 branch changes
   ``` 
4. Checkout the main branch, make changes and commit them
   ```shell
   git  checkout main

   git  commit -a -m "New changes before merge

   ```

5. After committing the changes to the **main** branch, it is the time to merge the changes from feature-2 branch
   ```shell
   git  merge feature-2
   ```
6. In this case a three way merge happen where git creates a common **merge commit** which is a parent of the last commits of the **main** and the **feature-2** branch
g
   

 