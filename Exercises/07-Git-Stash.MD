### Saving half-baked work items

At any point of Work in Progress, if you want to save your changes (not wanting to commit it as your work is not totally complete), you can use the stash command <br>

```
git stash #saves your present work items with a stash number
git stash save "Work in Progress 21 March 2025"
git stash list #shows all stashes currently stored for you
git stash apply stash@{1} #Apply stash numbered #1
git stash pop #Pops and removes the top-most stashed work & applies it

```