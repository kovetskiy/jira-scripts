Usage
=====
Run `jira-set-branch` for set current branch in current issue

Run `jira-now open` or just `jira-now` for open current issue in your
x-www-browser

Jira-now tricks
===============

``
git checkout -b feature-`jira-now print`-hottest
``

or if you want switch to branch of current issue (if exists)

``
git checkout `jira-now branch`
``

Add function to your bashrc/zshrc:

```
function gcof() {
    if [ ! -z $1 ]; then
        git checkout -b `jira-now print`-$1
    else
        git checkout `jira-now branch`
    fi
}
```

And use it
```
gcof shiiii
```
or just
```
gcof
```
