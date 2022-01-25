

# Quick Setup

## …or create a new repository on the command line
```
echo "# git-commander" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:umutyerebakmaz/git-commander.git
git push -u origin main
```

## …or push an existing repository from the command line

```
git remote add origin git@github.com:umutyerebakmaz/git-commander.git
git branch -M main
git push -u origin main
```

## how to delete all commit history in github?

1. Checkout
```
git checkout --orphan latest_branch
```

2. Add all the files
```
git add -A
```

3. Commit the changes
```
git commit -m "first commit"
```

4. Delete the branch
```
git branch -D main
```

5. Rename the current branch to main
```
git branch -m main
```

6. Finally, force update your repository
```
git push -f origin main
```

## how to delete all local git branches?
```
git branch -D `git branch --merged | grep -v \* | xargs`
```
or 
```
git branch --merged | grep -v \* | xargs git branch -D 
```

## how to delete given local git branch?

```
git branch -d local_branch_name
```
## License

The MIT License (MIT). Please see [License File](https://github.com/umutyerebakmaz/git-commander/blob/main/LICENCE) for more information.