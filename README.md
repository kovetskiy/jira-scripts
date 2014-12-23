Usage
=====
Run `jira-set-branch` for set current branch in current issue

Run `jira-now open` or just `jira-now` for open current issue in your
x-www-browser

Jira-now tricks
===============

``git checkout -b feature-`jira-now print`-hottest``

Add function to your bashrc/zshrc:

```
gcof() { git checkout -b `jira-now print`-$1 }
```

And use it
```
gcof shiiii
```
