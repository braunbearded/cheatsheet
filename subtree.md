# Subtree
Add other repos to yours by using subtree

## Add subtree as remote
git remote add -f reponame https://github.com/user-corp/repo1.git

## Add repo to your repo
Move in your root directory of the repo then run:

git subtree add --prefix repo/destination reponame master --squash

This will "clone" the content of your subtree repo in repo/destination. So it
won't create a new folder like git clone does.

## Update subtree
Be in your root directory of the repo then run:

git fetch reponame master
git subtree pull --prefix repo/destination reponame master --squash
