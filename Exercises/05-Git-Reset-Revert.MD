### Undoing Changes
Though Git has provisions to roll-back changes, it is always advisable not to go back in History unless & untill something is very critical.

#### Git Reset
This commands provides you 3 variations (Soft, Mixed & Hard) to un-do changes from Git History. Please refer to the following Git History of commits from a sample Repository, the top-most one is the recent commit and the bottom-most one is the first commit:
![](images/Reset.png?raw=true)

There are 3 ways to reset to any particular commit in History, say 4th Commit from the present one (as marked in the followed picture):
![](images/Reset1.png?raw=true)
* Soft Reset : Will un-do changes as per request but changes are retained and they are still present in Git Index
* Mixed Reset : This is the default option, and this is similar to Soft reset but the changes are removed from Git Index
* Hard Reset : Use this with caution as it will totally remove all changes that were made till that snapshot that is chosen

```
git reset --soft COMMIT_ID_OF_DESIRED_STATE
git reset --soft 9f1b24d6476af6304fd81a14096c6c243251a93b
git reset 9f1b24d6476af6304fd81a14096c6c243251a93b #Mixed Reset
git reset --hard 9f1b24d6476af6304fd81a14096c6c243251a93b #Will get rid of all changes this commit

git reset --soft HEAD^ #undo the last commit which typically rolls back one commit from the HEAD

git reset --soft HEAD^3 #Goes back 3 commits from the present Head
```

#### Git Revert

A better way of un-doing change is to add a new commit/change which un-does desirable change.This works on a commit by commit basis and can be applied for another number of commits, one after the other
```
git revert COMMIT_ID
# This will add a new commit (History goes forward) but this commit actually removes the changes done in COMMIT_ID
git revert COMMIT_ID1, COMMIT_ID2,... #A bunch of commits can also be taken care of one after the other but use this with caution
```
