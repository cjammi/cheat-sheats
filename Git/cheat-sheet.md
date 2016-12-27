# Git

## See files changed in a commit
```
git show --pretty="" --name-only <sha_of_C8>
git diff-tree --no-commit-id --name-only -r (sha_of_C8)
git diff <sha_of_C8>^ <sha_of_C8> [filename]
```


## Discard all un-staged changes
```
git checkout -- .
```

## See merges by an author
```
git log --merges --author james.bond@OO7.com
```

## delete local branch
```
git branch -d <local_branch_name>
```

## Branch:
```
git checkout <sha_of_C8>
git checkout -b <branch_name>
git branch -r
```

## Pull/Fetch:
```
git pull --rebase <remote name> <branch name>
git fetch --prune
git pull
```

## Commit:
```
git commit -a
git commit --dry-run
```

## ADD:
```
git add .
```

## RESET:
```
git reset --hard <sha_of_C8>
```

## REVERT:
```
git revert --no-edit -m 1 (sha_of_C8)
```


## PUSH:
```
git push origin <local_branch_name>
git push -u origin <remote_branch_name>
git push origin <local_branch_name>:<remote_branch_name>
```

## MERGE:
```
git merge <branch_to_be_merged_name> --no-edit
```

## CHERRY-PICK:
```
git cherry-pick (sha_of_C8)
```

## LOG:
```
git log --pretty=format:"%h %s" --graph
git log --graph  --decorate  --first-parent <local_branch_name>
git log <master_branch_name>..<slave_branch_name>   --oneline
```

## DIFF:
```
git remote show origin
git diff --name-only HEAD~1 HEAD
```