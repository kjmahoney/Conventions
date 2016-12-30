#Pushing to 2 (or more) repos
###Make sure you are a collaborator when performing this step

1. Create an `all` remote to your git

```
git remote add all GITHUBSSH.GIT
```

2. Add your repository to the `all` remote

```
git remote set-url --add --push all YOURORIGINALGITHUBREPO
```

3. Add another repository to the `all` remote

```
git remote set-url --add --push all ANYADDITIONALGITHUBREPOS
```

4. To push to both type `git push all`

```
git remote add all GITHUBSSH.GIT
```

***Optional
Renaming your `origin`

`git remote rename origin NEWNAME`
  
