# Merging

#### Merging branches using `git merge`

```bash
git merge master develop
# Merge the commits of the master branch to develop

git merge master
# Merge the commits of the master branch to your c urrent branch
```



#### Merging branches using `git rebase`
```bash
git checkout develop
git rebase master
# Integrate the commits of develop starting at the tip of your master branch.

git checkout develop
git rebase -i master
```