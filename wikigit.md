# Wikigit

- [Log](#log)
- [Status](#status)
- [Pull](#pull)
- [Commit](#commit)
- [Revert commit](#revert-commit)
- [Checkout to commit](#checkout-to-commit)
- [Stash](#stash)


---
<div id='log'/>

## Log

```cmd
git log
```
Show the commits history and some details.

---
<div id='pull'/>

## Pull

```cmd
git pull
git pull --merge
```
If you pull remote changes with the flag --merge, which is also the default, then your local changes are merged with the
remote changes. This results in a merge commit that points to the latest local commit and the latest remote commit.

---

```cmd
git pull --rebase
```
If you pull remote changes with the flag --rebase, then your local changes are reapplied on top of the remote changes.

---
<div id='commit'/>

## Commit

```cmd
git commit -m <"add commit message here..">
```
Do a commit.

---

```cmd
git commit -m <"add commit message here.."> --no-verify
git fcommit -m <"add commit message here..">
```
The flag --no-verify Avoid pre-commit checks.

---

<div id='revert-commit'/>

## Revert commit

```cmd
git revert <hash-commit>
```
Remove a specific commit.

---

<div id='checkout-to-commit'/>

## Checkout to commit

```cmd
git checkout <hash-commit>
```
Switch to specific commit.

---

<div id='stash'/>

## Stash

```cmd
git stash
git stash push
```
Save the local changes, reporting the state of the branch to the state of the HEAD commit.

---

```cmd
git stash save <"add a stash message here..">
```
Create a stash with a specific message.

---

```cmd
git stash list
```
Show the list of stashes. Example of result:

```cmd
output:
stash@{0}: On Nome_Branch: Messaggio..
```
{0} show the index assign to the specific stash

---

```cmd
git stash apply <stash@{0}>
```
Get a specific stash by index (stash@{0}).
NB. this stash won't delete.

---

```cmd
git stash drop <stash@{0}>
```
Remove a specific stash by index (stash@{0}).
NB. this command removes the stash without applying the change.

---

```cmd
git stash pop
```
Remove the stash at TOP position of the list.
NB.

---
