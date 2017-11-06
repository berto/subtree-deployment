# Deploying Multiple Heroku Apps

Here is an example of having multiple applications in the same repository deployed to Heroku.

NOTE: each sub-directory contains its own `package.json` 

# Step By Step

1. Create heroku applications and add remotes

```
heroku create -r heroku-v1
heroku create -r heroku-v2
heroku create -r heroku-v3
```

2. Push each app to heroku

```
git subtree push --prefix v1 heroku-v1 master
git subtree push --prefix v2 heroku-v2 master
git subtree push --prefix v3 heroku-v3 master
```
