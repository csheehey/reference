# reference

This project contains general-purpose scripts for reference.

## Git Process

1. In git bash (pc), clone the repo

```
git clone <enter repo address>
```

2. Then, navigate to the cloned repo, pull the latest changes from the originating branch and create the new branch.  Here, we branch (or fork) from the Main (master) branch.
```
cd chegg-event-spec/
git checkout main
git pull
git checkout -b <JIRA TICKET or name of new branch>
```

3. Add, save and commit changes
```
npm install (!only if you haven't previously installed npm)

atom (!or text editor of choice... save changes in project)

npm run build (!only when stitching together files in a build process)

git add <insert the name of the files/folders that have changed> (e.g., git add src/fields/my_new_field-v1.0.0.json) or git add -A if you want to live dangerously>

git commit -m "<JIRA TICKET> commit message"
```

4. Push changes to create new remote branch 
```
git push origin <JIRA TICKET or name of new branch>
```

5. Set upstream branch to track new remote branch from main
```
git push --set-upstream origin <JIRA TICKET or name of new branch>
```

6. Finally, go into git UI (or click on link from output of step 4) and create Merge Request
