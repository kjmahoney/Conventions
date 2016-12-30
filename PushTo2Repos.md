#Pushing to 2 (or more) github repos
###Make sure you are a collaborator when performing this step

1. Create an `all` remote to your git

```
git remote add all GITHUBSSH.GIT
```

3. Add your repository to the `all` remote

```
git remote set-url --add --push all YOURORIGINALGITHUBREPO
```

4. Add another repository to the `all` remote

```
git remote set-url --add --push all ANYADDITIONALGITHUBREPOS
```

4. To push to both type `git push all`


***

##Optional
Renaming your `origin`

`git remote rename origin NEWNAME`
  
