### Making changes to last commit (ONLY)

Minor mistakes in the last commit can be fixed using "--amend" flag <br>

Updates to the last commit (only the last one) can be made using 'git commit --amend' command <br>
* Commit message can be modified
* If you missed out adding any file(s) in the last commit, those can be updated as well

```
git commit -am "Defect #3458 fixed"
# The commit message contains incorrect defect number, let us fix it
git commit --amend -m "Defect #3456 fixed"
```

Including missed out files <br>
```
git commit -am "Fixed Issue #234"
# Forgot to add a source code file 'hello.py' in the previous commit
git add hello.py
git commit --amend --no-edit
# The --no-edit flag will allow you to make the amendment to your commit without changing its commit message

```